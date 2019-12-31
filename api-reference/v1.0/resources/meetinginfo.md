---
title: Тип ресурса Митингинфо
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ef003db89ea676b4415a90c27913add49aad6e1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913179"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="b742a-103">Тип ресурса Митингинфо</span><span class="sxs-lookup"><span data-stu-id="b742a-103">meetingInfo resource type</span></span>

<span data-ttu-id="b742a-104">Это абстрактный класс, который содержит сведения о собрании.</span><span class="sxs-lookup"><span data-stu-id="b742a-104">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="b742a-105">Чтобы присоединиться к существующему собранию, необходимо либо указать [организермитингинфо](organizermeetinginfo.md) в сочетании с [чатинфо](./chatinfo.md), либо только с [токенмитингинфо](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="b742a-105">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="b742a-106">Производные типы</span><span class="sxs-lookup"><span data-stu-id="b742a-106">Derived types</span></span>

| <span data-ttu-id="b742a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b742a-107">Type</span></span>                                                 | <span data-ttu-id="b742a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b742a-108">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="b742a-109">организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="b742a-109">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="b742a-110">Сведения об организаторе собрания</span><span class="sxs-lookup"><span data-stu-id="b742a-110">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="b742a-111">токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="b742a-111">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="b742a-112">Зашифрованный маркер, содержащий сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="b742a-112">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b742a-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b742a-113">JSON representation</span></span>

<span data-ttu-id="b742a-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b742a-114">The following is a JSON representation of the resource.</span></span>

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
