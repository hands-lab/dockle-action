# Dockle Action

![GitHub](https://img.shields.io/github/license/hands-lab/dockle-action)

<!-- TOC depthFrom:2 -->

- [Usage](#usage)
  - [Basic usage](#basic-usage)
  - [With optional parameters](#with-optional-parameters)
- [Inputs](#inputs)

<!-- /TOC -->

## Usage

### Basic usage

```yaml
steps:
  - uses: hands-lab/dockle-action@v1
    with:
      image: hello-world
```

### With optional parameters

```yaml
steps:
  - uses: hands-lab/dockle-action@v1
    with:
      image: hello-world
      exit-code: '1'
      exit-level: WARN
```

## Inputs

|Name|Type|Required|Default|Description|
|:--:|:--:|:--:|:--:|:--|
|image|string|True||image name|
|exit-code|string|False|'0'|exit code when alerts were found|
|exit-level|string|False|WARN|alert level (INFO, WARN, FATAL)|
