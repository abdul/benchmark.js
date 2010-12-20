# Benchmark
* [Benchmark.CALIBRATIONS](#static-CALIBRATIONS)
* [Benchmark.version](#static-version)
* [Benchmark.compare](#static-compare)
* [Benchmark.each](#static-each)
* [Benchmark.extend](#static-extend)
* [Benchmark.filter](#static-filter)
* [Benchmark.forIn](#static-forIn)
* [Benchmark.formatNumber](#static-formatNumber)
* [Benchmark.hasKey](#static-hasKey)
* [Benchmark.indexOf](#static-indexOf)
* [Benchmark.interpolate](#static-interpolate)
* [Benchmark.invoke](#static-invoke)
* [Benchmark.isArray](#static-isArray)
* [Benchmark.isCalibrated](#static-isCalibrated)
* [Benchmark.isClassOf](#static-isClassOf)
* [Benchmark.isHostType](#static-isHostType)
* [Benchmark.join](#static-join)
* [Benchmark.map](#static-map)
* [Benchmark.noop](#static-noop)
* [Benchmark.platform](#static-platform)
* [Benchmark.reduce](#static-reduce)
* [Benchmark.trim](#static-trim)

# Benchmark.prototype
* [Benchmark#CALIBRATION_INDEX](#CALIBRATION_INDEX)
* [Benchmark#CYCLE_DELAY](#CYCLE_DELAY)
* [Benchmark#DEFAULT_ASYNC](#DEFAULT_ASYNC)
* [Benchmark#DETECT_INFINITY](#DETECT_INFINITY)
* [Benchmark#INIT_RUN_COUNT](#INIT_RUN_COUNT)
* [Benchmark#MAX_TIME_ELAPSED](#MAX_TIME_ELAPSED)
* [Benchmark#MIN_TIME](#MIN_TIME)
* [Benchmark#MoE](#MoE)
* [Benchmark#RME](#RME)
* [Benchmark#SD](#SD)
* [Benchmark#SEM](#SEM)
* [Benchmark#aborted](#aborted)
* [Benchmark#count](#count)
* [Benchmark#cycles](#cycles)
* [Benchmark#error](#error)
* [Benchmark#hz](#hz)
* [Benchmark#persist](#persist)
* [Benchmark#running](#running)
* [Benchmark#times](#times)
* [Benchmark#times.cycle](#cycle)
* [Benchmark#times.elapsed](#elapsed)
* [Benchmark#times.period](#period)
* [Benchmark#times.start](#start)
* [Benchmark#times.stop](#stop)
* [Benchmark#abort](#abort)
* [Benchmark#addListener](#addListener)
* [Benchmark#clone](#clone)
* [Benchmark#emit](#emit)
* [Benchmark#removeAllListeners](#removeAllListeners)
* [Benchmark#removeListener](#removeListener)
* [Benchmark#reset](#reset)
* [Benchmark#run](#run)
* [Benchmark#toString](#toString)

# Benchmark
## <a name="static-CALIBRATIONS" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1356">Benchmark.CALIBRATIONS</a>
Benchmarks to establish iteration overhead.

## <a name="static-version" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1371">Benchmark.version</a>
The version number.

## <a name="static-compare" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L840">Benchmark.compare(other)</a>
Determines if the benchmark's hertz is higher than another.

### Arguments
1. `other` *(Object)*: The benchmark to compare.

### Returns
*(Number)*: Returns `1` if higher, `-1` if lower, and `0` if indeterminate.

## <a name="static-each" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L367">Benchmark.each(array, callback)</a>
A generic bare-bones Array#forEach solution.
Callbacks may terminate the loop by explicitly returning false.

### Arguments
1. `array` *(Array)*: The array to iterate over.
2. `callback` *(Function)*: The function called per iteration.

## <a name="static-extend" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L386">Benchmark.extend(destination, source)</a>
Copies source properties to the destination object.

### Arguments
1. `destination` *(Object)*: The destination object.
2. `[source={}]` *(Object)*: The source object.

### Returns
*(Object)*: The destination object.

## <a name="static-filter" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L401">Benchmark.filter(array, callback)</a>
A generic bare-bones Array#filter solution.

### Arguments
1. `array` *(Array)*: The array to iterate over.
2. `callback` *(Function)*: The function called per iteration.

### Returns
*(Array)*: A new array of values that passed callback filter.

## <a name="static-forIn" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L414">Benchmark.forIn(object, callback)</a>
A generic bare-bones for-in solution for an object's own properties.

### Arguments
1. `object` *(Object)*: The object to iterate over.
2. `callback` *(Function)*: The function called per iteration.

## <a name="static-formatNumber" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L429">Benchmark.formatNumber(number)</a>
Converts a number to a more readable comma separated string representation.

### Arguments
1. `number` *(Number)*: The number to convert.

### Returns
*(String)*: The more readable string representation.

## <a name="static-hasKey" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L447">Benchmark.hasKey(object, key)</a>
Checks if an object has the specified key as a direct property.

### Arguments
1. `object` *(Object)*: The object to check.
2. `key` *(String)*: The key to check for.

### Returns
*(Boolean)*: Returns true if key is a direct property, else false.

## <a name="static-indexOf" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L478">Benchmark.indexOf(array, value)</a>
A generic bare-bones Array#indexOf solution.

### Arguments
1. `array` *(Array)*: The array to iterate over.
2. `value` *(Mixed)*: The value to search for.

### Returns
*(Number)*: The index of the matched value or `-1`.

## <a name="static-interpolate" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L584">Benchmark.interpolate(string, object)</a>
Modify a string by replacing named tokens with matching object property values.

### Arguments
1. `string` *(String)*: The string to modify.
2. `object` *(Object)*: The template object.

### Returns
*(String)*: The modified string.

## <a name="static-invoke" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L497">Benchmark.invoke(benches, methodName, args)</a>
Invokes a given method, with arguments, on all benchmarks in an array.

### Arguments
1. `benches` *(Array)*: Array of benchmarks to iterate over.
2. `methodName` *(String|Object)*: Name of method to invoke or options object.
3. `args` *(Array)*: Arguments to invoke the method with.

## <a name="static-isArray" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L599">Benchmark.isArray(value)</a>
Determines if the given value is an array.

### Arguments
1. `value` *(Mixed)*: The value to check.

### Returns
*(Boolean)*: Returns true if value is an array, else false.

## <a name="static-isCalibrated" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L609">Benchmark.isCalibrated()</a>
Checks if calibration benchmarks have completed.

### Returns
*(Boolean)*: Returns true if calibrated, false if not.

## <a name="static-isClassOf" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L622">Benchmark.isClassOf(object, name)</a>
Checks if an object is of the specified class.

### Arguments
1. `object` *(Object)*: The object.
2. `name` *(String)*: The name of the class.

### Returns
*(Boolean)*: Returns true if of the class, else false.

## <a name="static-isHostType" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L636">Benchmark.isHostType(object, property)</a>
Host objects can return type values that are different from their actual
data type. The objects we are concerned with usually return non-primitive
types of object, function, or unknown.

### Arguments
1. `object` *(Mixed)*: The owner of the property.
2. `property` *(String)*: The property name to check.

### Returns
*(Boolean)*: Returns true if the property value is a non-primitive, else false.

## <a name="static-join" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L650">Benchmark.join(object, separator1, separator2)</a>
Creates a string of joined array values or object key-value pairs.

### Arguments
1. `object` *(Array|Object)*: The object to operate on.
2. `[separator1=',']` *(String)*: The separator used between key-value pairs.
3. `[separator2=': ']` *(String)*: The separator used between keys and values.

### Returns
*(String)*: The joined result.

## <a name="static-map" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L672">Benchmark.map(array, callback)</a>
A generic bare-bones Array#map solution.

### Arguments
1. `array` *(Array)*: The array to iterate over.
2. `callback` *(Function)*: The function called per iteration.

### Returns
*(Array)*: A new array of values returned by the callback.

## <a name="static-noop" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L684">Benchmark.noop()</a>
A no operation function.

## <a name="static-platform" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1214">Benchmark.platform</a>
Platform object containing browser name, version, and operating system.

## <a name="static-reduce" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L697">Benchmark.reduce(array, callback, accumulator)</a>
A generic bare-bones Array#reduce solution.

### Arguments
1. `array` *(Array)*: The array to iterate over.
2. `callback` *(Function)*: The function called per iteration.
3. `accumulator` *(Mixed)*: Initial value of the accumulator.

### Returns
*(Mixed)*: The accumulator.

## <a name="#{hash}" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1601">Benchmark#timesstop</a>
A timestamp of when the benchmark finished (ms).


# Benchmark.prototype
## <a name="CALIBRATION_INDEX" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1440">Benchmark#CALIBRATION_INDEX</a>
The index of the calibration benchmark to use when computing results.

## <a name="CYCLE_DELAY" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1447">Benchmark#CYCLE_DELAY</a>
The delay between test cycles (secs).

## <a name="DEFAULT_ASYNC" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1454">Benchmark#DEFAULT_ASYNC</a>
A flag to indicate methods will run asynchronously by default.

## <a name="DETECT_INFINITY" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1461">Benchmark#DETECT_INFINITY</a>
A flag to indicate protection against large run counts if Infinity ops/sec is detected.

## <a name="INIT_RUN_COUNT" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1468">Benchmark#INIT_RUN_COUNT</a>
The default number of times to execute a test on a benchmark's first cycle.

## <a name="MAX_TIME_ELAPSED" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1475">Benchmark#MAX_TIME_ELAPSED</a>
The maximum time a benchmark is allowed to run before finishing (secs).

## <a name="MIN_TIME" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1482">Benchmark#MIN_TIME</a>
The time needed to reduce the percent uncertainty of measurement to 1% (secs).

## <a name="MoE" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1489">Benchmark#MoE</a>
The margin of error.

## <a name="RME" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1496">Benchmark#RME</a>
The relative margin of error (expressed as a percentage of the mean).

## <a name="SD" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1503">Benchmark#SD</a>
The sample standard deviation.

## <a name="SEM" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1510">Benchmark#SEM</a>
The standard error of the mean.

## <a name="aborted" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1545">Benchmark#aborted</a>
A flag to indicate if the benchmark is aborted.

## <a name="count" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1517">Benchmark#count</a>
The number of times a test was executed.

## <a name="cycles" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1524">Benchmark#cycles</a>
The number of cycles performed while benchmarking.

## <a name="error" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1531">Benchmark#error</a>
The error object if the test failed.

## <a name="hz" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1538">Benchmark#hz</a>
The number of executions per second.

## <a name="persist" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1552">Benchmark#persist</a>
A flag to indicate if results persist for the browser session.

## <a name="running" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1559">Benchmark#running</a>
A flag to indicate if the benchmark is running.

## <a name="times" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1566">Benchmark#times</a>
An object of timing data including cycle, elapsed, period, start, and stop.

## <a name="cycle" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1573">Benchmark#times.cycle</a>
The time taken to complete the last cycle (secs)

## <a name="elapsed" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1580">Benchmark#times.elapsed</a>
The time taken to complete the benchmark (secs).

## <a name="period" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1587">Benchmark#times.period</a>
The time taken to execute the test once (secs).

## <a name="start" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1594">Benchmark#times.start</a>
A timestamp of when the benchmark started (ms).

## <a name="stop" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1601">Benchmark#times.stop</a>
A timestamp of when the benchmark finished (ms).

## <a name="abort" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L794">Benchmark#abort()</a>
Aborts the benchmark as well as in progress calibrations without recording times.

## <a name="addListener" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L724">Benchmark#addListener(type, listener)</a>
Registers a single listener of a specified event type.

### Arguments
1. `type` *(String)*: The event type.
2. `listener` *(Function)*: The function called when the event occurs.

### Returns
*(Object)*: The benchmark instance.

## <a name="clone" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L819">Benchmark#clone(options)</a>
Creates a cloned benchmark with the same test function and options.

### Arguments
1. `options` *(Object)*: Overwrite cloned options.

### Returns
*(Object)*: Cloned instance.

## <a name="emit" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L738">Benchmark#emit(type)</a>
Executes all registered listeners of a specified event type.

### Arguments
1. `type` *(String)*: The event type.

## <a name="removeAllListeners" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L779">Benchmark#removeAllListeners(type)</a>
Unregisters all listeners of a specified event type.

### Arguments
1. `type` *(String)*: The event type.

### Returns
*(Object)*: The benchmark instance.

## <a name="removeListener" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L761">Benchmark#removeListener(type, listener)</a>
Unregisters a single listener of a specified event type.

### Arguments
1. `type` *(String)*: The event type.
2. `listener` *(Function)*: The function to unregister.

### Returns
*(Object)*: The benchmark instance.

## <a name="reset" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L851">Benchmark#reset()</a>
Reset properties and abort if running.

## <a name="run" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L1178">Benchmark#run(async)</a>
Starts running the benchmark.

### Arguments
1. `[async=false]` *(Boolean)*: Flag to run asynchronously.

## <a name="toString" href="//github.com/mathiasbynens/benchmark.js/blob/master/benchmark.js#L888">Benchmark#toString()</a>
Displays relevant benchmark information when coerced to a string.