# Initiation à l'environnement C#/.NET

## Utilitaire .NET CLI

Il est nécessaire d'installer le SDK .NET pour avoir accès à la commande `dotnet`.

### Création d'un nouveau projet .NET à partir d'un template :

```
dotnet new <template>
```

### Ajout d'un package NuGet au projet .NET :

```
dotnet add package <package>
```

### Compilation du projet et de ses dépendences :

```
dotnet build
```

### Publication de l'application :

```
dotnet publish
```

### Création d'un package NuGet à partir du projet :

```
dotnet pack
```

### Démarrage de l'application à partir d'une DLL générée :

```
dotnet <dll>
```

### Démarrage de l'application sans compilation explicite :

```
dotnet run
```

### Démarrage d'un test unitaire :

```
dotnet test
```

### Nettoyage du projet :

```
dotnet clean
```

## Fichier de configuration `.csproj`

Il s'agit du fichier de configuration du projet au format XML.

Ce fichier définit :
- le type de la sortie de la compilation
- la version du Framework .NET à utiliser
- la cible de démarrage de l'application (au format `<namespace>.<classe>`)
- l'icône de l'application
- ...

Il est possible de configurer manuellement des packages NuGet à utiliser :

```xml
	<ItemGroup>
		<PackageReference Include="<package>" Version="<version>" />
	</ItemGroup>
```

Les ressources embarquées dans l'application sont également déclarées dans ce fichier :

```xml
<ItemGroup>
    <EmbeddedResource Include="<fichier>" />
</ItemGroup>
```

## Visual Studio

Visual Studio permet la configuration simple :
- du projet
- des packages NuGet
- des ressources
- ...
