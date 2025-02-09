<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [RunOptions](./bitburner.runoptions.md)

## RunOptions interface


**Signature:**

```typescript
interface RunOptions 
```

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [ramOverride?](./bitburner.runoptions.ramoverride.md) |  | number | <p>_(Optional)_ The RAM allocation to launch each thread of the script with.</p><p>Lowering this will <i>not</i> automatically let you get away with using less RAM: the dynamic RAM check enforces that all [NS](./bitburner.ns.md) functions actually called incur their cost. However, if you know that certain functions that are statically present (and thus included in the static RAM cost) will never be called in a particular circumstance, you can use this to avoid paying for them.</p><p>You can also use this to <i>increase</i> the RAM if the static RAM checker has missed functions that you need to call.</p><p>Must be greater-or-equal to the base RAM cost. Defaults to the statically calculated cost.</p> |
|  [temporary?](./bitburner.runoptions.temporary.md) |  | boolean | _(Optional)_ Whether this script is excluded from saves, defaults to false |
|  [threads?](./bitburner.runoptions.threads.md) |  | number | _(Optional)_ Number of threads that the script will run with, defaults to 1 |

