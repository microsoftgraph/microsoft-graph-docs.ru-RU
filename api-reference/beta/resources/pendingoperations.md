---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d83a68bf555fa5cc239fb38b147d12754f223e13
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333432"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="34ed6-103">Тип ресурса Пендингоператионс</span><span class="sxs-lookup"><span data-stu-id="34ed6-103">pendingOperations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34ed6-104">Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.</span><span class="sxs-lookup"><span data-stu-id="34ed6-104">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="34ed6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="34ed6-105">Properties</span></span>

| <span data-ttu-id="34ed6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="34ed6-106">Property</span></span>     | <span data-ttu-id="34ed6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="34ed6-107">Type</span></span>        | <span data-ttu-id="34ed6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="34ed6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34ed6-109">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="34ed6-109">pendingContentUpdate</span></span>|[<span data-ttu-id="34ed6-110">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="34ed6-110">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="34ed6-111">Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="34ed6-111">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34ed6-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34ed6-112">JSON representation</span></span>

<span data-ttu-id="34ed6-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34ed6-113">The following is a JSON representation of the resource.</span></span>

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
