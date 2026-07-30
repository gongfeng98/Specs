# lynx-family Specs

This repository stores the CocoaPods Specs for `lynx-family` components.

## Background

The `lynx-family` iOS components were originally published and indexed through the official CocoaPods `trunk`. Since `cocoapods trunk` is no longer maintained, this repository now serves as the self-hosted Specs source for managing and distributing Pod versions for `lynx-family` components.

## Usage

Add this Specs source to your project's `Podfile`:

```ruby
source 'https://github.com/lynx-family/Specs.git'
```

Then declare dependencies as usual:

```ruby
pod 'YourPodName', 'x.y.z'
```

Install dependencies:

```bash
pod install
```

## Publishing

When a new version of a `lynx-family` component is released, the corresponding `.podspec` should be pushed to this Specs repository. A typical workflow looks like this:

```bash
pod repo add lynx-family-specs https://github.com/lynx-family/Specs.git
pod repo push lynx-family-specs YourPodName.podspec
```

## Directory Structure

A Specs repository usually follows the standard CocoaPods directory layout:

```text
Specs/
└── YourPodName/
    └── x.y.z/
        └── YourPodName.podspec
```

