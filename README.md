Minimal Example of Bazel Plugin Reference Issue

Project 2 depends on project 1 as a JVM dep.  Project 1 is
brought in as a local repository in project 2's WORKSPACE
file.

Steps to reproduce:
1. Import Project 2 as a bazel project in Intellij with bazel 
   plugin installed
2. Run bazel sync
3. Go to project2/src/main/sample2/Sample2.scala and CTRL+B 
   Sample.sample() to follow reference to project1.sample.
   It will take you to decompiled code instead of source.
