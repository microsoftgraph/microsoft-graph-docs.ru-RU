---
title: Тип ресурса Организермитингинфо
description: 'Содержит сведения об организаторе собрания. '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 89f487b5edcf1b176a67d10b0ae45d8dd62c46d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447264"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="74316-103">Тип ресурса Организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="74316-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="74316-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="74316-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74316-105">Содержит сведения об организаторе собрания.</span><span class="sxs-lookup"><span data-stu-id="74316-105">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="74316-106">Чтобы присоединиться к существующему собранию, необходимо либо указать сочетание типов ресурсов Организермитингинфо и [чатинфо](./chatinfo.md) , либо сам тип ресурса [токенмитингинфо](./tokenmeetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="74316-106">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="74316-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74316-107">Properties</span></span>

| <span data-ttu-id="74316-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74316-108">Property</span></span>                     | <span data-ttu-id="74316-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74316-109">Type</span></span>                          | <span data-ttu-id="74316-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74316-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="74316-111">organizer</span><span class="sxs-lookup"><span data-stu-id="74316-111">organizer</span></span>                    | [<span data-ttu-id="74316-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="74316-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="74316-113">Удостоверение Azure Active Directory для организатора.</span><span class="sxs-lookup"><span data-stu-id="74316-113">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="74316-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74316-114">JSON representation</span></span>

<span data-ttu-id="74316-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74316-115">The following is a JSON representation of the resource.</span></span>

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
