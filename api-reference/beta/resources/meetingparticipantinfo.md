---
title: тип ресурса meetingParticipantInfo
description: Сведения о участнике собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 03d2c207d8c64d3e8b63dae223b624f575b193fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956955"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="d494f-103">тип ресурса meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="d494f-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="d494f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d494f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d494f-105">Содержит сведения о участнике собрания.</span><span class="sxs-lookup"><span data-stu-id="d494f-105">Contains information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d494f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d494f-106">Properties</span></span>

| <span data-ttu-id="d494f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d494f-107">Property</span></span> | <span data-ttu-id="d494f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d494f-108">Type</span></span>                          | <span data-ttu-id="d494f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d494f-109">Description</span></span>                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="d494f-110">identity</span><span class="sxs-lookup"><span data-stu-id="d494f-110">identity</span></span> | [<span data-ttu-id="d494f-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="d494f-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="d494f-112">Сведения о удостоверениях участника.</span><span class="sxs-lookup"><span data-stu-id="d494f-112">Identity information of the participant.</span></span>                                           |
| <span data-ttu-id="d494f-113">upn</span><span class="sxs-lookup"><span data-stu-id="d494f-113">upn</span></span>      | <span data-ttu-id="d494f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="d494f-114">String</span></span>                        | <span data-ttu-id="d494f-115">Основное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="d494f-115">User principal name of the participant.</span></span>                                            |
| <span data-ttu-id="d494f-116">role</span><span class="sxs-lookup"><span data-stu-id="d494f-116">role</span></span>     | <span data-ttu-id="d494f-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="d494f-117">onlineMeetingRole</span></span>             | <span data-ttu-id="d494f-118">Указывает роль участника собрания.</span><span class="sxs-lookup"><span data-stu-id="d494f-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="d494f-119">Возможные значения `attendee` , `presenter` и `producer` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d494f-119">Possible values are `attendee`, `presenter`, `producer`, and `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d494f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d494f-120">JSON representation</span></span>

<span data-ttu-id="d494f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d494f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
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


