---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 31629ee29bc91b3b2bae53e954743df17cde7d30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521971"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="2c931-103">Тип ресурса Пендингоператионс</span><span class="sxs-lookup"><span data-stu-id="2c931-103">pendingOperations resource type</span></span>

<span data-ttu-id="2c931-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c931-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c931-105">Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.</span><span class="sxs-lookup"><span data-stu-id="2c931-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="2c931-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c931-106">Properties</span></span>

| <span data-ttu-id="2c931-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c931-107">Property</span></span>     | <span data-ttu-id="2c931-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2c931-108">Type</span></span>        | <span data-ttu-id="2c931-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2c931-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c931-110">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="2c931-110">pendingContentUpdate</span></span>|[<span data-ttu-id="2c931-111">пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="2c931-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="2c931-112">Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="2c931-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c931-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c931-113">JSON representation</span></span>

<span data-ttu-id="2c931-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c931-114">The following is a JSON representation of the resource.</span></span>

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
