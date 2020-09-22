---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a4c9e350d75783208a14310605540ab110f64f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971669"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="421e9-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="421e9-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="421e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="421e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="421e9-105">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="421e9-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="421e9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="421e9-106">Properties</span></span>

| <span data-ttu-id="421e9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="421e9-107">Property</span></span>       | <span data-ttu-id="421e9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="421e9-108">Type</span></span>                          | <span data-ttu-id="421e9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="421e9-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="421e9-110">хищения</span><span class="sxs-lookup"><span data-stu-id="421e9-110">identity</span></span>       | [<span data-ttu-id="421e9-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="421e9-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="421e9-112">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="421e9-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="421e9-113">Основное</span><span class="sxs-lookup"><span data-stu-id="421e9-113">upn</span></span>            | <span data-ttu-id="421e9-114">String</span><span class="sxs-lookup"><span data-stu-id="421e9-114">String</span></span>                        | <span data-ttu-id="421e9-115">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="421e9-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="421e9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="421e9-116">JSON representation</span></span>

<span data-ttu-id="421e9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421e9-117">The following is a JSON representation of the resource.</span></span>

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


