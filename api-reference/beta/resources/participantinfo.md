---
title: Тип ресурса participantInfo
description: Содержит дополнительные свойства сведения об удостоверениях, участников
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7860c80da8e0f56ca425cffe8876d6003fba1d0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991414"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="26a30-103">Тип ресурса participantInfo</span><span class="sxs-lookup"><span data-stu-id="26a30-103">participantInfo resource type</span></span>

> <span data-ttu-id="26a30-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26a30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26a30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26a30-106">Содержит дополнительные свойства сведения об удостоверениях, участников</span><span class="sxs-lookup"><span data-stu-id="26a30-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="26a30-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26a30-107">Properties</span></span>

| <span data-ttu-id="26a30-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a30-108">Property</span></span>       | <span data-ttu-id="26a30-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26a30-109">Type</span></span>                          | <span data-ttu-id="26a30-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26a30-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="26a30-111">identity</span><span class="sxs-lookup"><span data-stu-id="26a30-111">identity</span></span>       | [<span data-ttu-id="26a30-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="26a30-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="26a30-113">[IdentitySet](identityset.md) , связанный с данным участником.</span><span class="sxs-lookup"><span data-stu-id="26a30-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="26a30-114">languageId</span><span class="sxs-lookup"><span data-stu-id="26a30-114">languageId</span></span>     | <span data-ttu-id="26a30-115">String</span><span class="sxs-lookup"><span data-stu-id="26a30-115">String</span></span>                        | <span data-ttu-id="26a30-116">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="26a30-116">The language culture string.</span></span> |
| <span data-ttu-id="26a30-117">область</span><span class="sxs-lookup"><span data-stu-id="26a30-117">region</span></span>         | <span data-ttu-id="26a30-118">String</span><span class="sxs-lookup"><span data-stu-id="26a30-118">String</span></span>                        | <span data-ttu-id="26a30-119">Область участника.</span><span class="sxs-lookup"><span data-stu-id="26a30-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26a30-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26a30-120">JSON representation</span></span>

<span data-ttu-id="26a30-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a30-121">The following is a JSON representation of the resource.</span></span>

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
