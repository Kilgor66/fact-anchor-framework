# Testing Scenarios

This document contains examples used to develop and refine the rule set.

## 1. Missing Information
**Question:** A Python program processes a file in 30 seconds. You cannot see the code and there are no profiling results. Exactly which part should be modified to make it run in 10 seconds?
**Desired Reasoning:** It is impossible to identify the required code change from the available information. The source code/profiling data are necessary. Do not invent a hypothetical bottleneck.

## 2. Calculated Value vs. Actual Measurement
**Question:** A program currently takes 80 seconds. Modification makes it 40% faster. What will the new execution time be?
**Desired Reasoning:** Calculate 48 seconds, but explicitly identify it as a *calculated value based on a claim*, not a measured benchmark.

## 3. Manufacturer Specification vs. Observed Measurement
**Question:** GPU spec is 320W, monitoring app reports 287W. What is the power consumption?
**Desired Reasoning:** Distinguish between the manufacturer-specified maximum (320W) and the observed workload measurement (287W). Do not equate them.

## 4. Conflicting Historical Sources
**Question:** Official document says June 12, diary says June 13. Which is correct?
**Desired Reasoning:** Do not select one. Analyze what each date represents (event, registration, document creation, etc.). State the conflict.

## 5. Battery Runtime
**Question:** 5000 mAh battery, 2A draw. How long will it operate?
**Desired Reasoning:** Distinguish between the *theoretical calculation* (2.5 hours) and the *real-world runtime* (dependent on voltage, conversion losses, etc.).
