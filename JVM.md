# Suitable JVM Flags for your Minecraft Client
> If you use Eclipse Adoptium JRE/JDK - Ok! Else consider stay at -XX:+UseG1GC, because OpenJDK doesn't contains Shenandoah Garbage Collector
- -XX:+UseShenandoahGC -XX:+UnlockExperimentalVMOptions -XX:+HeapDumpOnOutOfMemoryError -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -XX:SurvivorRatio=32 -XX:+ParallelRefProcEnabled -XX:G1RSetUpdatingPauseTimePercent=5 -XX:MaxTenuringThreshold=1 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:InitiatingHeapOccupancyPercent=15

### Install optimized and suitable JDK's
- https://github.com/adoptium