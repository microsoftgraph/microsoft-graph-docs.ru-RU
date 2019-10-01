---
title: пендингконтентупдате
description: Ресурс Пендингконтентупдате указывает на то, что операция, которая может повлиять на двоичный контент driveItem, ожидает завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1637ac3faa1d42cd47f49735a1b24fb60868a23d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333433"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="59de2-103">Тип ресурса Пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="59de2-103">pendingContentUpdate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59de2-104">Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="59de2-104">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="59de2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="59de2-105">Properties</span></span>

| <span data-ttu-id="59de2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="59de2-106">Property</span></span>     | <span data-ttu-id="59de2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="59de2-107">Type</span></span>         | <span data-ttu-id="59de2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="59de2-108">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="59de2-109">куеуеддатетиме</span><span class="sxs-lookup"><span data-stu-id="59de2-109">queuedDateTime</span></span>|<span data-ttu-id="59de2-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59de2-110">DateTimeOffset</span></span>|<span data-ttu-id="59de2-111">Дата и время, когда отложенная двоичная операция была поставлена в очередь в течение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="59de2-111">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="59de2-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59de2-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59de2-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59de2-113">JSON representation</span></span>

<span data-ttu-id="59de2-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59de2-114">The following is a JSON representation of the resource.</span></span>

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
