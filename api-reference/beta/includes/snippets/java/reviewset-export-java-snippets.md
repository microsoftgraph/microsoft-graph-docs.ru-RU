---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f49ef72eeea5d934b074a53de731b37346067a76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772880"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String outputName = "2020-12-06 Contoso investigation export";

String description = "Export for the Contoso investigation";

EnumSet<ExportOptions> exportOptions = EnumSet.of(ExportOptions.ORIGINAL_FILES,ExportOptions.FILE_INFO,ExportOptions.TAGS);

ExportFileStructure exportStructure = ExportFileStructure.DIRECTORY;

graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").reviewSets("e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc")
    .export(outputName,description,null,null,exportOptions,exportStructure)
    .buildRequest()
    .post();

```