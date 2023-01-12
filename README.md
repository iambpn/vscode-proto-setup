# vscode-proto-setup
Guide on how to setup Proto syntax and error highlight in vscode

---

Steps:
1. Install vscode extension: [vsode-proto3](https://marketplace.visualstudio.com/items?itemName=zxh404.vscode-proto3)
2. Install protoc compiler: [protoc](https://grpc.io/docs/protoc-installation/)
3. Under `.vscode` folder `settings.json` add following: [Link to StackOverflow](https://stackoverflow.com/questions/68276704/proto-importing-the-proto-file-in-vscode-got-not-found-error-by-ide)
   ```json
   "protoc": {
      // need to add this to remove import error in proto file
      "options": [
        "--proto_path=<proto folders>"
      ]
    }
   ```
