# extensions
## extensions list
```bat
> code --list-extensions >> vs_code_extensions_list.txt

ansenhuang.vscode-view-readme
dbaeumer.vscode-eslint
dracula-theme.theme-dracula
EditorConfig.EditorConfig
formulahendry.code-runner
jpoissonnier.vscode-styled-components
marlon407.code-groovy
mikestead.dotenv
naumovs.color-highlight
octref.vetur
Pivotal.vscode-boot-dev-pack
Pivotal.vscode-concourse
Pivotal.vscode-manifest-yaml
Pivotal.vscode-spring-boot
PKief.material-icon-theme
redhat.java
redhat.vscode-xml
ritwickdey.LiveServer
rocketseat.rocketseatreactjs
rocketseat.rocketseatreactnative
VisualStudioExptTeam.vscodeintellicode
vscjava.vscode-java-debug
vscjava.vscode-java-dependency
vscjava.vscode-java-pack
vscjava.vscode-java-test
vscjava.vscode-maven
vscjava.vscode-spring-boot-dashboard
vscjava.vscode-spring-initializr
znck.vue

```

## install
```bat
> cat vs_code_extensions_list.txt | xargs -n 1 code --install-extensions
```

## settings.json
```json
{
    "workbench.iconTheme": "material-icon-theme",
    "workbench.colorTheme": "Dracula",

    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },

    "files.associations": {
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    ".prettierrc": "json"
    },

    "emmet.syntaxProfiles": { "javascript": "jsx" },
    "emmet.includeLanguages": { "javascript": "javascriptreact" },

    "material-icon-theme.folders.associations": {
        "infra": "app",
        "entities": "class",
        "schemas": "class",
        "typeorm": "database",
        "repositories": "mappings",
        "http": "container",
        "migrations": "tools",
        "modules": "components",
        "implementations": "core",
        "dtos": "typescript",
        "fakes": "mock",
        "websockets": "pipe",
        "protos": "pipe",
        "grpc": "pipe"
    },

    "material-icon-theme.files.associations": {
        "ormconfig.json": "database",
        "tsconfig.json": "tune",
        "*.proto": "3d"
    },

    "workbench.startupEditor": "newUntitledFile",
    "editor.suggestSelection": "first",
    "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
    
    "java.home": "/usr/lib/jvm/java-11-openjdk-amd64",
    "java.completion.enabled": true,
    "java.configuration.runtimes": [
        {
            "name": "JavaSE-1.8",
            "path": "/usr/lib/jvm/java-8-openjdk-amd64",
            "default": true
        },
        {
            "name": "JavaSE-11",
            "path": "/usr/lib/jvm/java-11-openjdk-amd64"
        }
    ],
}
```