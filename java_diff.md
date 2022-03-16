
# New features
## JAVA 11
**Oracle Vs Open JDK**

Java 10 was the last free **Oracle JDK release that we could use commercially without a license.Starting with Java 11, there's no free long-term support (LTS) from Oracle**.
Thankfully, **Oracle continues to provide Open JDK releases, which we can download and use without charge.**

**The Not Predicate Method**

**New String Methods** — strip(), stripLeading(),stripTrailing(),isBlank(),lines(),repeat(n)

**A No-Op Garbage Collector**

A new garbage collector called Epsilon is available for use in Java 11 as an experimental feature.
It's called a No-Op (no operations) because it allocates memory but does not actually collect any garbage. Thus, Epsilon is applicable for simulating out of memory errors.
Obviously Epsilon won't be suitable for a typical production Java application; however, there are a few specific use-cases where it could be useful:
Performance testing
Memory pressure testing
VM interface testing and
Extremely short-lived jobs
In order to enable it, use the -XX:+UnlockExperimentalVMOptions -XX:+UseEpsilonGC flag.

**Decommission JAXB**

**Local-Variable Syntax for Lambda Parameters** 

(x, y) -> x.process(y)
We’ll be able to write:
(var x, var y) -> x.process(y)

## JAVA 12
**Switch Expressions** – Classic switch statement:
STRING RESULT = SWITCH (DAY) {
CASE "M", "W", "F" -> "MWF";
CASE "T", "TH", "S" -> "TTS";
DEFAULT -> {
IF(DAY.ISEMPTY())
BREAK "PLEASE INSERT A VALID DAY.";
ELSE
BREAK "LOOKS LIKE A SUNDAY.";
}
};

**File mismatch() Method** – i.e. long mismatch = Files.mismatch(filePath1, filePath2);

**Java Strings New Methods** : indent, transform,describeConstable, resolveConstantDesc.


