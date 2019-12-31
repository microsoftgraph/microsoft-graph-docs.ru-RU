---
title: Тип ресурса Организермитингинфо
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e7750e282801a938fd42c01717cc7bbbedcf95a3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913683"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="5674d-103">Тип ресурса Организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="5674d-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="5674d-104">Содержит сведения об организаторе собрания.</span><span class="sxs-lookup"><span data-stu-id="5674d-104">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="5674d-105">Чтобы присоединиться к существующему собранию, необходимо либо указать сочетание типов ресурсов Организермитингинфо и [чатинфо](./chatinfo.md) , либо сам тип ресурса [токенмитингинфо](./tokenmeetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="5674d-105">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="5674d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5674d-106">Properties</span></span>

| <span data-ttu-id="5674d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5674d-107">Property</span></span>                     | <span data-ttu-id="5674d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5674d-108">Type</span></span>                          | <span data-ttu-id="5674d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5674d-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="5674d-110">organizer</span><span class="sxs-lookup"><span data-stu-id="5674d-110">organizer</span></span>                    | [<span data-ttu-id="5674d-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="5674d-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="5674d-112">Удостоверение Azure Active Directory для организатора.</span><span class="sxs-lookup"><span data-stu-id="5674d-112">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5674d-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5674d-113">JSON representation</span></span>

<span data-ttu-id="5674d-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5674d-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
