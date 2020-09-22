---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 20f74cb3bd812371a1b18d479452e94521ae622c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020526"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="b9ab1-103">Тип ресурса Пендингоператионс</span><span class="sxs-lookup"><span data-stu-id="b9ab1-103">pendingOperations resource type</span></span>

<span data-ttu-id="b9ab1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9ab1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9ab1-105">Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.</span><span class="sxs-lookup"><span data-stu-id="b9ab1-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="b9ab1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9ab1-106">Properties</span></span>

| <span data-ttu-id="b9ab1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ab1-107">Property</span></span>                | <span data-ttu-id="b9ab1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ab1-108">Type</span></span>        | <span data-ttu-id="b9ab1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ab1-109">Description</span></span> |
|:------------------------|:------------|:------------|
|<span data-ttu-id="b9ab1-110">**пендингконтентупдате**</span><span class="sxs-lookup"><span data-stu-id="b9ab1-110">**pendingContentUpdate**</span></span> |[<span data-ttu-id="b9ab1-111">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="b9ab1-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="b9ab1-112">Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="b9ab1-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9ab1-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9ab1-113">JSON representation</span></span>

<span data-ttu-id="b9ab1-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ab1-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->

