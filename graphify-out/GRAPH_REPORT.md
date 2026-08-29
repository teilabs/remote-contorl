# Graph Report - remote-control  (2026-08-29)

## Corpus Check
- Corpus is ~10,065 words - fits in a single context window. You may not need a graph.

## Summary
- 269 nodes · 573 edges · 22 communities (21 shown, 1 thin omitted)
- Extraction: 92% EXTRACTED · 8% INFERRED · 0% AMBIGUOUS · INFERRED: 45 edges (avg confidence: 0.81)
- Token cost: 3,720 input · 4,611 output

## Community Hubs (Navigation)
- Android Control UI
- Android Activity Lifecycle
- Models and Tests
- Server Configuration Parsing
- Signed HTTP Client
- Architecture and Security Docs
- Server Request Execution
- MDPI Round Launcher
- XXHDPI Launcher Assets
- XXXHDPI Launcher Assets
- XXXHDPI Round Launcher
- Gradle Wrapper Script
- HDPI Launcher Assets
- HDPI Round Launcher
- MDPI Launcher Assets
- XHDPI Launcher Assets
- XHDPI Round Launcher
- XXHDPI Round Launcher
- Java Package Namespace

## God Nodes (most connected - your core abstractions)
1. `MainActivity` - 51 edges
2. `AppConfig` - 24 edges
3. `RemoteArgument` - 21 edges
4. `RemoteCommand` - 17 edges
5. `CommandArgument` - 17 edges
6. `SyncableControl` - 12 edges
7. `RemoteClient` - 12 edges
8. `SigningKeyStore` - 12 edges
9. `ArgumentValue` - 11 edges
10. `CommandExecutor` - 11 edges

## Surprising Connections (you probably didn't know these)
- `Ed25519 Request Signing` --semantically_similar_to--> `Ed25519 Request Authentication`  [INFERRED] [semantically similar]
  android/README.md → README.md
- `Device-Bound Credential Protection` --conceptually_related_to--> `Android Keystore`  [INFERRED]
  android/README.md → README.md
- `MainActivity` --references--> `SigningKeyStore`  [EXTRACTED]
  android/app/src/main/java/io/github/teilabs/remote/android/MainActivity.java → android/app/src/main/java/io/github/teilabs/remote/android/SigningKeyStore.java
- `App` --references--> `AppConfig`  [EXTRACTED]
  server/src/main/java/io/github/teilabs/remote/App.java → server/src/main/java/io/github/teilabs/remote/config/AppConfig.java
- `CommandDescriptor` --references--> `CommandArgument`  [EXTRACTED]
  server/src/main/java/io/github/teilabs/remote/App.java → server/src/main/java/io/github/teilabs/remote/config/CommandArgument.java

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Signed Protected Request Flow** — readme_android_client, readme_ed25519_request_authentication, readme_android_keystore, readme_protected_http_endpoints [EXTRACTED 1.00]
- **Remote Command Metadata Flow** — readme_javalin_server, readme_command_metadata, readme_android_client, readme_configured_command [EXTRACTED 1.00]

## Communities (22 total, 1 thin omitted)

### Community 0 - "Android Control UI"
Cohesion: 0.09
Nodes (17): ArgumentValue, RemoteValueSetter, SyncableControl, RemoteArgument, RemoteCommand, android.view.View, android.widget.EditText, android.widget.Spinner (+9 more)

### Community 1 - "Android Activity Lifecycle"
Cohesion: 0.12
Nodes (12): MainActivity, android.content.SharedPreferences, android.os.Bundle, android.os.Handler, android.widget.ImageButton, android.widget.LinearLayout, android.widget.ProgressBar, android.widget.TextView (+4 more)

### Community 2 - "Models and Tests"
Cohesion: 0.10
Nodes (14): ExampleInstrumentedTest, ExampleUnitTest, androidx.test.ext.junit.runners.AndroidJUnit4, org.junit.rules.TemporaryFolder, org.junit.runner.RunWith, org.junit.Test, ArgumentType, SELECT (+6 more)

### Community 3 - "Server Configuration Parsing"
Cohesion: 0.15
Nodes (10): com.fasterxml.jackson.databind.JsonNode, com.fasterxml.jackson.databind.ObjectMapper, Ed25519PublicKeyParameters, org.bouncycastle.crypto.params.Ed25519PublicKeyParameters, AppConfig, Command, CommandType, SIMPLE (+2 more)

### Community 4 - "Signed HTTP Client"
Cohesion: 0.14
Nodes (5): ExecutionResult, RemoteClient, SigningKeyStore, android.content.Context, javax.crypto.SecretKey

### Community 5 - "Architecture and Security Docs"
Cohesion: 0.09
Nodes (24): Android Emulator Host Routing, Android Keystore, Connection Settings, Device-Bound Credential Protection, Ed25519 Request Signing, Remote Android, Server Command Metadata, Server app.json Configuration (+16 more)

### Community 6 - "Server Request Execution"
Cohesion: 0.21
Nodes (6): io.javalin.http.Context, App, CommandDescriptor, CommandExecutor, ExecutionResult, UnknownCommandException

### Community 7 - "MDPI Round Launcher"
Cohesion: 0.50
Nodes (4): Android Robot Symbol, Circular Icon Border, Green Grid Background, Round Android App Launcher Icon

### Community 8 - "XXHDPI Launcher Assets"
Cohesion: 0.50
Nodes (4): Android Robot Symbol, Green Grid Background, Android App Launcher Icon, Rounded Square Icon Frame

### Community 9 - "XXXHDPI Launcher Assets"
Cohesion: 0.50
Nodes (4): Android Launcher Icon, Diagonal Robot Shadow, Green Square Grid Background, White Android Robot Head

### Community 10 - "XXXHDPI Round Launcher"
Cohesion: 0.50
Nodes (4): Android Robot Symbol, Circular Icon Border, Green Grid Background, Round Android App Launcher Icon

### Community 11 - "Gradle Wrapper Script"
Cohesion: 0.83
Nodes (3): gradlew script, die(), warn()

### Community 12 - "HDPI Launcher Assets"
Cohesion: 0.67
Nodes (3): Android Robot Symbol, Green Grid Background, Android App Launcher Icon

### Community 13 - "HDPI Round Launcher"
Cohesion: 1.00
Nodes (3): White Android Robot Head Symbol, Green Globe Grid Background, Round Android Launcher Icon

### Community 14 - "MDPI Launcher Assets"
Cohesion: 0.67
Nodes (3): Android Launcher Icon, White Android Robot Head, Green Grid Background

### Community 15 - "XHDPI Launcher Assets"
Cohesion: 1.00
Nodes (3): White Android Robot Head Symbol, Green Grid Background, Android Launcher Icon

### Community 16 - "XHDPI Round Launcher"
Cohesion: 0.67
Nodes (3): Green Circular Grid Background, Round Android Launcher Icon, White Android Robot Head

### Community 17 - "XXHDPI Round Launcher"
Cohesion: 1.00
Nodes (3): White Android Robot Head Symbol, Green Globe Grid Background, Round Android Launcher Icon

## Knowledge Gaps
- **28 isolated node(s):** `io.github.teilabs:remote`, `SLIDER`, `TEXT`, `SELECT`, `TOGGLE` (+23 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `MainActivity` connect `Android Activity Lifecycle` to `Android Control UI`, `Signed HTTP Client`?**
  _High betweenness centrality (0.096) - this node is a cross-community bridge._
- **Why does `CommandArgument` connect `Models and Tests` to `Server Configuration Parsing`, `Server Request Execution`?**
  _High betweenness centrality (0.037) - this node is a cross-community bridge._
- **Why does `AppConfig` connect `Server Configuration Parsing` to `Models and Tests`, `Server Request Execution`?**
  _High betweenness centrality (0.033) - this node is a cross-community bridge._
- **What connects `io.github.teilabs:remote`, `SLIDER`, `TEXT` to the rest of the system?**
  _28 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Android Control UI` be split into smaller, more focused modules?**
  _Cohesion score 0.09387755102040816 - nodes in this community are weakly interconnected._
- **Should `Android Activity Lifecycle` be split into smaller, more focused modules?**
  _Cohesion score 0.12051282051282051 - nodes in this community are weakly interconnected._
- **Should `Models and Tests` be split into smaller, more focused modules?**
  _Cohesion score 0.10476190476190476 - nodes in this community are weakly interconnected._