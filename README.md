# realworld
RealWorld OSS Angular Frontend and Java Spring Backend for training purposes.

# Backend instructions
Go to the backend folder and run the following commands:

JDK 25 is required to run the backend. You can download it from [Adoptium](https://adoptium.net/).

Gradle wrapper is included in the project, so you can run Gradle tasks without installing Gradle globally. If you encounter a permission denied error when running Gradle tasks, run `chmod +x gradlew` to grant execution permission.

```bash
./gradlew clean :realworld:bootRun
```

# Frontend instructions
Go to the frontend folder and run the following commands:

bun is required to run the frontend. You can download it from [Bun](https://bun.sh/).

```bash
bun run setup
bun run start
``` 


