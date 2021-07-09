DataWeave - Support 2.3.0
===========

## Patches Release Notes

| Issue | Description |
|----------------|----------------|
|**SE-15904**| Fixes CSE reducing two expression without taking into account middle nodes. |
|**SE-15918**| Adding support for escaped char sequences on settings.|
|**SE-16292**| Json with spaces after array value was failing in in-memory parser.|
|**SE-16389**| Nested Dynamic Objects is skipping elements.|
|**SE-16381**| Add an alternative migration to date - date for 4.3.x|
|**SE-16431**| Cache compiled expressions based on string script|
|**SE-16468**| Map with value null should not be ignored|
|**SE-15453**| Includes a new property to handle the escaping of `>` in the XML module.|
|**SE-16915**| Remove troubleshooting log mistakenly introduced as part of SE-16389.|
|**SE-16539**| Fixes error while parsing JSON with whitespaces between array elements. |
|**SE-15894**| Json Binary is not encoded into string the same way as 2.1.x|
|**SE-16462**| Single Key Value Pair was not parsed correctly when mixed with conditional|
|**SE-16620**| Avro Should take into account logical types for conversion of types|
|**SE-16534**| Adding support for mule.verbose.exceptions to print DW addintional stacktrace exception|
|**SE-15362**| Fixes NPE in XML module.|
|**SE-15249**| Attribute selector not dispatching to the correct implementation|
|**SE-15834**| Don't store the inferred type as outputMimetype but as a property. So that TypedValues always return the typed value.|
|**DW-184**  | Write function should keep the correct mimeType and also keep the original inferred mimeType|
|**SE-17193**| Fix deployment freeze when having several nested function calls such as ++|
|**SE-16350**| When using `header=false` with `bodyStartLineNumber` CSV reader skips lines|
|**SE-17392**| Internal exception should never go out of service.| 
|**SE-16883**| Fix `causedBy` does not have the correct type defined for `Error`.|
|**SE-17570**| Avoid `StackOverflow` when using `some` and `every` with big arrays.|
|**SE-17520**| Selecting key named `$` was not working as expected.|
|**SE-9907** | Fixes `java.util.Timezone` not working as expected.|
|**SE-15970**| Fixes the `diff` function which was inverting the expected versus actual comparison.|
|**SE-17446**| DataWeave now ignores empty lines in Excel correctly.|
|**SE-17149**| In Excel, the number of cells read per row is now always at least the same as the header size, even if they are empty.|
|**SE-17773**|Add a system property `com.mulesoft.dw.valueSelector.selectsAlwaysFirst` that avoid caching the selected index.|
|**SE-17873**|Fix error while converting Instant to LocalDateTime with Min and Max|
|**FV-820**| Fix classloader leak on value provider on default value on function parameters|
|**FV-833**| Fix joinBy body doesn't validate against signature|
|**SE-14220**| Fixes `NullPointerException` in the FlatFile module.|
|**SE-16596**| Fixes `null` values not being transformed as all zeroes in hexadecimal in the Flat file module.|
|**DW-240**| Update EDI parser to latest version (2.3.10) in the Flat file module.|
|**SE-16372**| Make CSV streaming support BOM|
|**DW-289**| Upserting an object it was duplicating key value pairs in some cases|
|**SE-18393**| Detect correctly when a variable needs to be materialized with multiple if else|
|**SE-18136**| Excel reader maintain the position of the headers when there are some empty headers|
|**SE-18580**| Fix pattern matcher shouldn't require a new line|
|**DW-306**| Attributes should be accesible on update selector update|
|**DW-307**|Fix XML Comments not working on streaming mode|
|**SE-18882**|Fix substringBefore and substringBeforeLast|
|**DW-325**|NDJson was not working when being executed in parallel|
|**SE-19086**| Fix batching a streaming not working with deferred mode|
|**SE-19000**| Adding a new reader property called `tableLimit` to control the boundaries of where to read data Options are: 'HeaderSize', 'Unbounded' or The column Name.|
|**SE-19040**|Avoid throwing `NullPointerException` when the message of the exception is `null`.|
|**SE-13423**|Fix flatfile can't write dw keys as values.|
|**SE-19094**|Foreach with batchsize causing StreamClose|
|**DW-371**|Fix reader properties.|
|**SE-17677**|BinaryValue read buffer is now configurable with property com.mulesoft.dw.buffersize|
|**SE-17411**|Added support for `numeric literal` values at `Value Clause` when auto-generate FlatFile schemas from imported Cobol Copybook structures.|
|**SE-19157**|Splitter is generating the wrong exception that causes Scala Serialization issues.|
|**SE-19266**| Use the encoding when converting the string to byte array.|
|**SE-15159**|Includes a new property to handle DTD in XML module.| 
|**DW-375**| Avoid overflow by getting a binary token offset.| 
|**SE-19090**| Local imported modules are being cached.| 
|**SE-19442**| Fixing pattern matcher not working with comments.| 
|**SE-19846**| Remove resource from when close eager to avoid OOM|
|**SE-20005**| Increase the amount of namespaces that can be handled on indexed XML|
|**SE-19257**| Fixed the implementation of recordParsing, the lenient behavior is now able to handle shorter or longer records|
|**SE-20129**| Character reader property with value 'null' should be taken as empty value.|
|**SE-20372**| Avoid stackoverflow on StreamCapable Check recursive functions|
|**SE-20300**| Avoid OutOfMemory when using MultiPart.|
|**DW-377**| Disable DTD support by default. Use system property `com.mulesoft.dw.xml.supportDTD` or XML reader property `supportDtd` to change behaviour.|
