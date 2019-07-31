---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 62843378d53774d19ad3428e6b52c985761edda2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009771"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="acb2c-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="acb2c-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acb2c-104">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="acb2c-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="acb2c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="acb2c-105">Properties</span></span>

| <span data-ttu-id="acb2c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="acb2c-106">Property</span></span>       | <span data-ttu-id="acb2c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="acb2c-107">Type</span></span>                          | <span data-ttu-id="acb2c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="acb2c-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="acb2c-109">хищения</span><span class="sxs-lookup"><span data-stu-id="acb2c-109">identity</span></span>       | [<span data-ttu-id="acb2c-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="acb2c-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="acb2c-111">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="acb2c-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="acb2c-112">Основное</span><span class="sxs-lookup"><span data-stu-id="acb2c-112">upn</span></span>            | <span data-ttu-id="acb2c-113">String</span><span class="sxs-lookup"><span data-stu-id="acb2c-113">String</span></span>                        | <span data-ttu-id="acb2c-114">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="acb2c-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="acb2c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acb2c-115">JSON representation</span></span>

<span data-ttu-id="acb2c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acb2c-116">The following is a JSON representation of the resource.</span></span>

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
