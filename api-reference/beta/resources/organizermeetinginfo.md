---
title: Тип ресурса Организермитингинфо
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 210dfecb6252091663aeb981fcf82e2b3535dcac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998427"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="901b2-103">Тип ресурса Организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="901b2-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="901b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="901b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="901b2-105">Содержит сведения об организаторе собрания.</span><span class="sxs-lookup"><span data-stu-id="901b2-105">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="901b2-106">Чтобы присоединиться к существующему собранию, необходимо либо указать сочетание типов ресурсов Организермитингинфо и [чатинфо](./chatinfo.md) , либо сам тип ресурса [токенмитингинфо](./tokenmeetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="901b2-106">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="901b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="901b2-107">Properties</span></span>

| <span data-ttu-id="901b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="901b2-108">Property</span></span>                     | <span data-ttu-id="901b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="901b2-109">Type</span></span>                          | <span data-ttu-id="901b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="901b2-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="901b2-111">organizer</span><span class="sxs-lookup"><span data-stu-id="901b2-111">organizer</span></span>                    | [<span data-ttu-id="901b2-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="901b2-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="901b2-113">Удостоверение Azure Active Directory для организатора.</span><span class="sxs-lookup"><span data-stu-id="901b2-113">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="901b2-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="901b2-114">JSON representation</span></span>

<span data-ttu-id="901b2-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="901b2-115">The following is a JSON representation of the resource.</span></span>

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


