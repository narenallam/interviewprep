// After reviewing the code, I made the below changes and updated the file.
//
// Review Comments:
// - Deeply nested loops, instead should return early
// - Slicing is prefered than tuple unpacking assignments
// - lac of basic documentation(comments)
// - variable names or too short to understand at first glance
// - lengthy lines (more than 120 chars), wrapping and beatification required
// - excessive use of 'panic()', should handle the errors in higher order functions
// - Modularization and should think of reusability, should write as many functions
//   as possible, and should be open for extention(handling multiple text formats)
// - Idea of this tool has potenital for parallelism, where golang shines
// - command line help should be improved alot and user freidnly, as user has no idea
// - logging should be implemented as user doesn't want to see, dev messages
// - writing basic unittests, ensures the quality
//
// Final thougths:
// I made changes to the main.go file, modularized the code, implemented logging,
// took the advanatge of concurrent design of golang, implemented parallelism, and
// the bench marks are promising. It is nearly 4 times faster than the
// sequential version(depends on core count). We can run parallel version '-j=true' command option.
// Memory mangement, still can be improved. Algorithm can be improved by caching the
// results in a temp file.
//
