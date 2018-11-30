---
title: Тип ресурса participantInfo
description: Содержит дополнительные свойства сведения об удостоверениях, участников
ms.openlocfilehash: c6f429e353d80ea53c5f5c00ca084ae7a8a4a7c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074891"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="e2e5a-103">Тип ресурса participantInfo</span><span class="sxs-lookup"><span data-stu-id="e2e5a-103">participantInfo resource type</span></span>

> <span data-ttu-id="e2e5a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2e5a-106">Содержит дополнительные свойства сведения об удостоверениях, участников</span><span class="sxs-lookup"><span data-stu-id="e2e5a-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="e2e5a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2e5a-107">Properties</span></span>

| <span data-ttu-id="e2e5a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2e5a-108">Property</span></span>       | <span data-ttu-id="e2e5a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e2e5a-109">Type</span></span>                          | <span data-ttu-id="e2e5a-110">Description</span><span class="sxs-lookup"><span data-stu-id="e2e5a-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="e2e5a-111">identity</span><span class="sxs-lookup"><span data-stu-id="e2e5a-111">identity</span></span>       | [<span data-ttu-id="e2e5a-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="e2e5a-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="e2e5a-113">[IdentitySet](identityset.md) , связанный с данным участником.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="e2e5a-114">languageId</span><span class="sxs-lookup"><span data-stu-id="e2e5a-114">languageId</span></span>     | <span data-ttu-id="e2e5a-115">String</span><span class="sxs-lookup"><span data-stu-id="e2e5a-115">String</span></span>                        | <span data-ttu-id="e2e5a-116">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-116">The language culture string.</span></span> |
| <span data-ttu-id="e2e5a-117">область</span><span class="sxs-lookup"><span data-stu-id="e2e5a-117">region</span></span>         | <span data-ttu-id="e2e5a-118">String</span><span class="sxs-lookup"><span data-stu-id="e2e5a-118">String</span></span>                        | <span data-ttu-id="e2e5a-119">Область участника.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2e5a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2e5a-120">JSON representation</span></span>

<span data-ttu-id="e2e5a-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2e5a-121">The following is a JSON representation of the resource.</span></span>

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