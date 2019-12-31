---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 30b3ef3b3acd4f1cdaa7c7a0b4c63b4d8104c09b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913389"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="d119e-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="d119e-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d119e-104">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="d119e-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d119e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d119e-105">Properties</span></span>

| <span data-ttu-id="d119e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d119e-106">Property</span></span>       | <span data-ttu-id="d119e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d119e-107">Type</span></span>                          | <span data-ttu-id="d119e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d119e-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="d119e-109">хищения</span><span class="sxs-lookup"><span data-stu-id="d119e-109">identity</span></span>       | [<span data-ttu-id="d119e-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="d119e-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="d119e-111">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="d119e-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="d119e-112">Основное</span><span class="sxs-lookup"><span data-stu-id="d119e-112">upn</span></span>            | <span data-ttu-id="d119e-113">String</span><span class="sxs-lookup"><span data-stu-id="d119e-113">String</span></span>                        | <span data-ttu-id="d119e-114">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="d119e-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d119e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d119e-115">JSON representation</span></span>

<span data-ttu-id="d119e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d119e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
