---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2775dd3af7940f9022b9e7090125ed52fce397d6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006636"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="1c9a3-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="1c9a3-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c9a3-104">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="1c9a3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c9a3-105">Properties</span></span>

| <span data-ttu-id="1c9a3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c9a3-106">Property</span></span>       | <span data-ttu-id="1c9a3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1c9a3-107">Type</span></span>                          | <span data-ttu-id="1c9a3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1c9a3-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="1c9a3-109">хищения</span><span class="sxs-lookup"><span data-stu-id="1c9a3-109">identity</span></span>       | [<span data-ttu-id="1c9a3-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="1c9a3-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="1c9a3-111">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="1c9a3-112">Основное</span><span class="sxs-lookup"><span data-stu-id="1c9a3-112">upn</span></span>            | <span data-ttu-id="1c9a3-113">String</span><span class="sxs-lookup"><span data-stu-id="1c9a3-113">String</span></span>                        | <span data-ttu-id="1c9a3-114">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1c9a3-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c9a3-115">JSON representation</span></span>

<span data-ttu-id="1c9a3-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-116">The following is a JSON representation of the resource.</span></span>

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
