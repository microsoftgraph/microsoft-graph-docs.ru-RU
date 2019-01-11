---
title: Тип ресурса participantInfo
description: Содержит дополнительные свойства сведения об удостоверениях, участников
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 94bbc587f26f8b5122571899eb235d9c1fc27e90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870667"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="40993-103">Тип ресурса participantInfo</span><span class="sxs-lookup"><span data-stu-id="40993-103">participantInfo resource type</span></span>

> <span data-ttu-id="40993-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40993-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40993-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40993-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40993-106">Содержит дополнительные свойства сведения об удостоверениях, участников</span><span class="sxs-lookup"><span data-stu-id="40993-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="40993-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40993-107">Properties</span></span>

| <span data-ttu-id="40993-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40993-108">Property</span></span>       | <span data-ttu-id="40993-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40993-109">Type</span></span>                          | <span data-ttu-id="40993-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40993-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="40993-111">identity</span><span class="sxs-lookup"><span data-stu-id="40993-111">identity</span></span>       | [<span data-ttu-id="40993-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="40993-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="40993-113">[IdentitySet](identityset.md) , связанный с данным участником.</span><span class="sxs-lookup"><span data-stu-id="40993-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="40993-114">languageId</span><span class="sxs-lookup"><span data-stu-id="40993-114">languageId</span></span>     | <span data-ttu-id="40993-115">Строка</span><span class="sxs-lookup"><span data-stu-id="40993-115">String</span></span>                        | <span data-ttu-id="40993-116">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="40993-116">The language culture string.</span></span> |
| <span data-ttu-id="40993-117">область</span><span class="sxs-lookup"><span data-stu-id="40993-117">region</span></span>         | <span data-ttu-id="40993-118">Строка</span><span class="sxs-lookup"><span data-stu-id="40993-118">String</span></span>                        | <span data-ttu-id="40993-119">Область участника.</span><span class="sxs-lookup"><span data-stu-id="40993-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="40993-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40993-120">JSON representation</span></span>

<span data-ttu-id="40993-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40993-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
