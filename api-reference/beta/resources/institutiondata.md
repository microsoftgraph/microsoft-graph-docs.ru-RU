---
title: Тип ресурса Институтиондата
description: Тип ресурса Институтиондата
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a0734966d8a92aef5cd515043047bfcade35df47
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495447"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="f2e08-103">Тип ресурса Институтиондата</span><span class="sxs-lookup"><span data-stu-id="f2e08-103">institutionData resource type</span></span>

<span data-ttu-id="f2e08-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f2e08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2e08-105">Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="f2e08-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f2e08-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2e08-106">Properties</span></span>

| <span data-ttu-id="f2e08-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2e08-107">Property</span></span>     | <span data-ttu-id="f2e08-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f2e08-108">Type</span></span>                                 | <span data-ttu-id="f2e08-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2e08-109">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2e08-110">description</span><span class="sxs-lookup"><span data-stu-id="f2e08-110">description</span></span>   |<span data-ttu-id="f2e08-111">String</span><span class="sxs-lookup"><span data-stu-id="f2e08-111">String</span></span>                                |<span data-ttu-id="f2e08-112">Краткое описание учебного заведения, в котором пользователь изучается.</span><span class="sxs-lookup"><span data-stu-id="f2e08-112">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="f2e08-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f2e08-113">displayName</span></span>   |<span data-ttu-id="f2e08-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f2e08-114">String</span></span>                                |<span data-ttu-id="f2e08-115">Имя учреждения, в котором пользователь изучается.</span><span class="sxs-lookup"><span data-stu-id="f2e08-115">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="f2e08-116">location</span><span class="sxs-lookup"><span data-stu-id="f2e08-116">location</span></span>      |[<span data-ttu-id="f2e08-117">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f2e08-117">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="f2e08-118">Адрес или расположение института.</span><span class="sxs-lookup"><span data-stu-id="f2e08-118">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="f2e08-119">webUrl</span><span class="sxs-lookup"><span data-stu-id="f2e08-119">webUrl</span></span>        |<span data-ttu-id="f2e08-120">String</span><span class="sxs-lookup"><span data-stu-id="f2e08-120">String</span></span>                                |<span data-ttu-id="f2e08-121">Ссылка на домашнюю страницу "учреждение" или "Отдел".</span><span class="sxs-lookup"><span data-stu-id="f2e08-121">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="f2e08-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2e08-122">JSON representation</span></span>

<span data-ttu-id="f2e08-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2e08-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->