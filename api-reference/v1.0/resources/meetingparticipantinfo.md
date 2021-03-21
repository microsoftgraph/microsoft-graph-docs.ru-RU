---
title: тип ресурса meetingParticipantInfo
description: Сведения о участнике собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40209354f1621839bd51a20fcbafa4cd58b4fd8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962457"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="b218f-103">тип ресурса meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="b218f-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="b218f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b218f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b218f-105">Сведения о участнике собрания.</span><span class="sxs-lookup"><span data-stu-id="b218f-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="b218f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b218f-106">Properties</span></span>

| <span data-ttu-id="b218f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b218f-107">Property</span></span> | <span data-ttu-id="b218f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b218f-108">Type</span></span>                          | <span data-ttu-id="b218f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b218f-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="b218f-110">identity</span><span class="sxs-lookup"><span data-stu-id="b218f-110">identity</span></span> | [<span data-ttu-id="b218f-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="b218f-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="b218f-112">Сведения о удостоверениях участника.</span><span class="sxs-lookup"><span data-stu-id="b218f-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="b218f-113">upn</span><span class="sxs-lookup"><span data-stu-id="b218f-113">upn</span></span>      | <span data-ttu-id="b218f-114">String</span><span class="sxs-lookup"><span data-stu-id="b218f-114">String</span></span>                        | <span data-ttu-id="b218f-115">Основное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="b218f-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="b218f-116">role</span><span class="sxs-lookup"><span data-stu-id="b218f-116">role</span></span>     | <span data-ttu-id="b218f-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="b218f-117">onlineMeetingRole</span></span>             | <span data-ttu-id="b218f-118">Указывает роль участника собрания.</span><span class="sxs-lookup"><span data-stu-id="b218f-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="b218f-119">Возможные значения: `attendee`, `presenter` и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b218f-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b218f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b218f-120">JSON representation</span></span>

<span data-ttu-id="b218f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b218f-121">The following is a JSON representation of the resource.</span></span>

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

