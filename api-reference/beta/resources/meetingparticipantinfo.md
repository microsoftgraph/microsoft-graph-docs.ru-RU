---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635200"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="8a921-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="8a921-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="8a921-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a921-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a921-105">Содержит сведения о участнике собрания.</span><span class="sxs-lookup"><span data-stu-id="8a921-105">Contains information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="8a921-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a921-106">Properties</span></span>

| <span data-ttu-id="8a921-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a921-107">Property</span></span> | <span data-ttu-id="8a921-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8a921-108">Type</span></span>                          | <span data-ttu-id="8a921-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a921-109">Description</span></span>                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="8a921-110">хищения</span><span class="sxs-lookup"><span data-stu-id="8a921-110">identity</span></span> | [<span data-ttu-id="8a921-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a921-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="8a921-112">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="8a921-112">Identity information of the participant.</span></span>                                           |
| <span data-ttu-id="8a921-113">Основное</span><span class="sxs-lookup"><span data-stu-id="8a921-113">upn</span></span>      | <span data-ttu-id="8a921-114">String</span><span class="sxs-lookup"><span data-stu-id="8a921-114">String</span></span>                        | <span data-ttu-id="8a921-115">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a921-115">User principal name of the participant.</span></span>                                            |
| <span data-ttu-id="8a921-116">role</span><span class="sxs-lookup"><span data-stu-id="8a921-116">role</span></span>     | <span data-ttu-id="8a921-117">онлинемитингроле</span><span class="sxs-lookup"><span data-stu-id="8a921-117">onlineMeetingRole</span></span>             | <span data-ttu-id="8a921-118">Указывает роль участника в собрании.</span><span class="sxs-lookup"><span data-stu-id="8a921-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="8a921-119">Возможные значения: `attendee`, `presenter` и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8a921-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="8a921-120">значения Онлинемитингроле</span><span class="sxs-lookup"><span data-stu-id="8a921-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="8a921-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8a921-121">Value</span></span>              | <span data-ttu-id="8a921-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8a921-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="8a921-123">attendee</span><span class="sxs-lookup"><span data-stu-id="8a921-123">attendee</span></span>           | <span data-ttu-id="8a921-124">Участник является участником.</span><span class="sxs-lookup"><span data-stu-id="8a921-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="8a921-125">докладчика</span><span class="sxs-lookup"><span data-stu-id="8a921-125">presenter</span></span>          | <span data-ttu-id="8a921-126">Участник является выступающим.</span><span class="sxs-lookup"><span data-stu-id="8a921-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="8a921-127">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8a921-127">unknownFutureValue</span></span> | <span data-ttu-id="8a921-128">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="8a921-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="8a921-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a921-129">JSON representation</span></span>

<span data-ttu-id="8a921-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a921-130">The following is a JSON representation of the resource.</span></span>

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


