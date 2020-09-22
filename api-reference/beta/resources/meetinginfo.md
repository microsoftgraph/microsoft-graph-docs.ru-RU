---
title: Тип ресурса Митингинфо
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2330fe401ed0f220792bbf0de38bfb92b2aade28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971673"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="e4bdc-103">Тип ресурса Митингинфо</span><span class="sxs-lookup"><span data-stu-id="e4bdc-103">meetingInfo resource type</span></span>

<span data-ttu-id="e4bdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4bdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4bdc-105">Это абстрактный класс, который содержит сведения о собрании.</span><span class="sxs-lookup"><span data-stu-id="e4bdc-105">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="e4bdc-106">Чтобы присоединиться к существующему собранию, необходимо либо указать [организермитингинфо](organizermeetinginfo.md) в сочетании с [чатинфо](./chatinfo.md), либо только с [токенмитингинфо](tokenmeetinginfo.md).</span><span class="sxs-lookup"><span data-stu-id="e4bdc-106">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="e4bdc-107">Производные типы</span><span class="sxs-lookup"><span data-stu-id="e4bdc-107">Derived types</span></span>

| <span data-ttu-id="e4bdc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4bdc-108">Type</span></span>                                                 | <span data-ttu-id="e4bdc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4bdc-109">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="e4bdc-110">организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="e4bdc-110">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="e4bdc-111">Сведения об организаторе собрания</span><span class="sxs-lookup"><span data-stu-id="e4bdc-111">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="e4bdc-112">токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="e4bdc-112">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="e4bdc-113">Зашифрованный маркер, содержащий сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="e4bdc-113">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e4bdc-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4bdc-114">JSON representation</span></span>

<span data-ttu-id="e4bdc-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4bdc-115">The following is a JSON representation of the resource.</span></span>

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


