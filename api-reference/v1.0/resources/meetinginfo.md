---
title: Тип ресурса Митингинфо
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e777de1b9f6710156106ce8dab5704613b98e1e5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871393"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="c31ea-103">Тип ресурса Митингинфо</span><span class="sxs-lookup"><span data-stu-id="c31ea-103">meetingInfo resource type</span></span>

<span data-ttu-id="c31ea-104">Это абстрактный класс, который содержит сведения о собрании.</span><span class="sxs-lookup"><span data-stu-id="c31ea-104">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="c31ea-105">Чтобы присоединиться к существующему собранию, необходимо либо указать [организермитингинфо](organizermeetinginfo.md) в сочетании с [чатинфо](./chatinfo.md), либо только с [токенмитингинфо](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="c31ea-105">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="c31ea-106">Производные типы</span><span class="sxs-lookup"><span data-stu-id="c31ea-106">Derived types</span></span>

| <span data-ttu-id="c31ea-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c31ea-107">Type</span></span>                                                 | <span data-ttu-id="c31ea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c31ea-108">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="c31ea-109">организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="c31ea-109">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="c31ea-110">Сведения об организаторе собрания</span><span class="sxs-lookup"><span data-stu-id="c31ea-110">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="c31ea-111">токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="c31ea-111">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="c31ea-112">Зашифрованный маркер, содержащий сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="c31ea-112">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c31ea-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c31ea-113">JSON representation</span></span>

<span data-ttu-id="c31ea-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c31ea-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
