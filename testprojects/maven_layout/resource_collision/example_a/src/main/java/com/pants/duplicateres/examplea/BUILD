# Copyright 2014 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

jvm_binary(name='examplea',
  main='com.pants.duplicateres.examplea.Main',
  dependencies=[
    ':lib',
    ],
)

java_library(name='lib',
  sources=['Main.java'],
  resources=['testprojects/maven_layout/resource_collision/example_a/src/main/resources'],
  dependencies=[
    'testprojects/maven_layout/resource_collision/example_b/src/main/java/com/pants/duplicateres/exampleb:lib',
    'testprojects/maven_layout/resource_collision/lib/src/main/java/com/pants/duplicateres/lib',
  ],
)
