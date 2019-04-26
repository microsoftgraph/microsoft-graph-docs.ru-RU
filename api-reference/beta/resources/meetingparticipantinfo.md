---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3df338760bd1d2ff74cc79c706944c9b5fa7104d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342396"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="9b25f-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="9b25f-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b25f-104">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="9b25f-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9b25f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b25f-105">Properties</span></span>

| <span data-ttu-id="9b25f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b25f-106">Property</span></span>       | <span data-ttu-id="9b25f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9b25f-107">Type</span></span>                          | <span data-ttu-id="9b25f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9b25f-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="9b25f-109">хищения</span><span class="sxs-lookup"><span data-stu-id="9b25f-109">identity</span></span>       | [<span data-ttu-id="9b25f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="9b25f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="9b25f-111">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="9b25f-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="9b25f-112">Основное</span><span class="sxs-lookup"><span data-stu-id="9b25f-112">upn</span></span>            | <span data-ttu-id="9b25f-113">String</span><span class="sxs-lookup"><span data-stu-id="9b25f-113">String</span></span>                        | <span data-ttu-id="9b25f-114">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b25f-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9b25f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b25f-115">JSON representation</span></span>

<span data-ttu-id="9b25f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b25f-116">The following is a JSON representation of the resource.</span></span>

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
