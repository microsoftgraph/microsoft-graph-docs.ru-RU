---
title: Тип ресурса Организермитингинфо
description: 'Содержит сведения об организаторе собрания. '
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cdb23ebfe16822e4caa4374fbc8e21697533c7cc
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006608"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="bd71b-103">Тип ресурса Организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="bd71b-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd71b-104">Содержит сведения об организаторе собрания.</span><span class="sxs-lookup"><span data-stu-id="bd71b-104">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="bd71b-105">Чтобы присоединиться к существующему собранию, необходимо либо указать сочетание типов ресурсов Организермитингинфо и [чатинфо](./chatinfo.md) , либо сам тип ресурса [токенмитингинфо](./tokenmeetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="bd71b-105">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="bd71b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd71b-106">Properties</span></span>

| <span data-ttu-id="bd71b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd71b-107">Property</span></span>                     | <span data-ttu-id="bd71b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bd71b-108">Type</span></span>                          | <span data-ttu-id="bd71b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd71b-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="bd71b-110">organizer</span><span class="sxs-lookup"><span data-stu-id="bd71b-110">organizer</span></span>                    | [<span data-ttu-id="bd71b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="bd71b-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="bd71b-112">Удостоверение Azure Active Directory для организатора.</span><span class="sxs-lookup"><span data-stu-id="bd71b-112">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bd71b-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd71b-113">JSON representation</span></span>

<span data-ttu-id="bd71b-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd71b-114">The following is a JSON representation of the resource.</span></span>

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
