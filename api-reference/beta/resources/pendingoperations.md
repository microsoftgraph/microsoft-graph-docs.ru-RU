---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7b5d162bfcc9cccdfc7a2ea769e4ea39272e2d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998097"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="1eb0f-103">Тип ресурса Пендингоператионс</span><span class="sxs-lookup"><span data-stu-id="1eb0f-103">pendingOperations resource type</span></span>

<span data-ttu-id="1eb0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb0f-105">Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.</span><span class="sxs-lookup"><span data-stu-id="1eb0f-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="1eb0f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1eb0f-106">Properties</span></span>

| <span data-ttu-id="1eb0f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1eb0f-107">Property</span></span>     | <span data-ttu-id="1eb0f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1eb0f-108">Type</span></span>        | <span data-ttu-id="1eb0f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb0f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1eb0f-110">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="1eb0f-110">pendingContentUpdate</span></span>|[<span data-ttu-id="1eb0f-111">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="1eb0f-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="1eb0f-112">Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="1eb0f-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1eb0f-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1eb0f-113">JSON representation</span></span>

<span data-ttu-id="1eb0f-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1eb0f-114">The following is a JSON representation of the resource.</span></span>

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


