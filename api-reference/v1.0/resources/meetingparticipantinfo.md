---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742001"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="b6661-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="b6661-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="b6661-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6661-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6661-105">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="b6661-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="b6661-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6661-106">Properties</span></span>

| <span data-ttu-id="b6661-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6661-107">Property</span></span> | <span data-ttu-id="b6661-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6661-108">Type</span></span>                          | <span data-ttu-id="b6661-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6661-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="b6661-110">хищения</span><span class="sxs-lookup"><span data-stu-id="b6661-110">identity</span></span> | [<span data-ttu-id="b6661-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="b6661-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="b6661-112">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="b6661-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="b6661-113">Основное</span><span class="sxs-lookup"><span data-stu-id="b6661-113">upn</span></span>      | <span data-ttu-id="b6661-114">String</span><span class="sxs-lookup"><span data-stu-id="b6661-114">String</span></span>                        | <span data-ttu-id="b6661-115">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6661-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="b6661-116">role</span><span class="sxs-lookup"><span data-stu-id="b6661-116">role</span></span>     | <span data-ttu-id="b6661-117">онлинемитингроле</span><span class="sxs-lookup"><span data-stu-id="b6661-117">onlineMeetingRole</span></span>             | <span data-ttu-id="b6661-118">Указывает роль участника в собрании.</span><span class="sxs-lookup"><span data-stu-id="b6661-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="b6661-119">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b6661-119">Possible values are listed in the following table.</span></span> |

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="b6661-120">значения Онлинемитингроле</span><span class="sxs-lookup"><span data-stu-id="b6661-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="b6661-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6661-121">Value</span></span>              | <span data-ttu-id="b6661-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b6661-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="b6661-123">attendee</span><span class="sxs-lookup"><span data-stu-id="b6661-123">attendee</span></span>           | <span data-ttu-id="b6661-124">Участник является участником.</span><span class="sxs-lookup"><span data-stu-id="b6661-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="b6661-125">докладчика</span><span class="sxs-lookup"><span data-stu-id="b6661-125">presenter</span></span>          | <span data-ttu-id="b6661-126">Участник является выступающим.</span><span class="sxs-lookup"><span data-stu-id="b6661-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="b6661-127">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="b6661-127">unknownFutureValue</span></span> | <span data-ttu-id="b6661-128">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="b6661-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="b6661-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6661-129">JSON representation</span></span>

<span data-ttu-id="b6661-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6661-130">The following is a JSON representation of the resource.</span></span>

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

