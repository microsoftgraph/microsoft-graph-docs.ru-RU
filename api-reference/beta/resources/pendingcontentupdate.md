---
title: пендингконтентупдате
description: Ресурс Пендингконтентупдате указывает на то, что операция, которая может повлиять на двоичный контент driveItem, ожидает завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5e7291ac4591ba63bec96108dd46bf9561358bb4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998096"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="6a506-103">Тип ресурса Пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="6a506-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="6a506-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a506-105">Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="6a506-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="6a506-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a506-106">Properties</span></span>

| <span data-ttu-id="6a506-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a506-107">Property</span></span>     | <span data-ttu-id="6a506-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6a506-108">Type</span></span>         | <span data-ttu-id="6a506-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6a506-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="6a506-110">куеуеддатетиме</span><span class="sxs-lookup"><span data-stu-id="6a506-110">queuedDateTime</span></span>|<span data-ttu-id="6a506-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a506-111">DateTimeOffset</span></span>|<span data-ttu-id="6a506-112">Дата и время, когда отложенная двоичная операция была поставлена в очередь в течение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6a506-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="6a506-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a506-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a506-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a506-114">JSON representation</span></span>

<span data-ttu-id="6a506-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a506-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->


