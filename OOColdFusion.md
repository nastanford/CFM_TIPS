# Object Oriented ColdFusion

## Examples
[Adrian Moreno Code Examples](https://adrianmoreno.com/2007/08/23/object-oriented-coldfusion-1-intro-to-objectcfc.html)

#### Basic Tag Object 

```
<cfcomponent output="false" name="Object" hint="Simple CF Object">
  <cffunction name="init" access="public" output="false" returntype="Object" hint="constructor">
    <cfreturn this />
  </cffunction>
</cfcomponent>
```

```
<cfset obj = createObject("component", "Object").init() />
```

```
<cfinvoke component="Object" method="init" returnVariable="obj" />
```

