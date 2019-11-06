---
title: Тип ресурса Рекордоператион
description: Тип Рекордоператион
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 22b1fbd157b6b13d0b839a898440ee289aa2ec73
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006559"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="2f376-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="2f376-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f376-104">Тип Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="2f376-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="2f376-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f376-105">Properties</span></span>

| <span data-ttu-id="2f376-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f376-106">Property</span></span>                       | <span data-ttu-id="2f376-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2f376-107">Type</span></span>                        | <span data-ttu-id="2f376-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2f376-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2f376-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="2f376-109">clientContext</span></span>                  | <span data-ttu-id="2f376-110">String</span><span class="sxs-lookup"><span data-stu-id="2f376-110">String</span></span>                      | <span data-ttu-id="2f376-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="2f376-111">Unique Client Context string.</span></span> <span data-ttu-id="2f376-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="2f376-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="2f376-113">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="2f376-113">completionReason</span></span>               | <span data-ttu-id="2f376-114">String</span><span class="sxs-lookup"><span data-stu-id="2f376-114">String</span></span>                      | <span data-ttu-id="2f376-115">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="2f376-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="2f376-116">id</span><span class="sxs-lookup"><span data-stu-id="2f376-116">id</span></span>                             | <span data-ttu-id="2f376-117">Строка</span><span class="sxs-lookup"><span data-stu-id="2f376-117">String</span></span>                      | <span data-ttu-id="2f376-118">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f376-118">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2f376-119">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="2f376-119">recordingAccessToken</span></span>           | <span data-ttu-id="2f376-120">String</span><span class="sxs-lookup"><span data-stu-id="2f376-120">String</span></span>                      | <span data-ttu-id="2f376-121">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="2f376-121">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="2f376-122">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="2f376-122">recordingLocation</span></span>              | <span data-ttu-id="2f376-123">String</span><span class="sxs-lookup"><span data-stu-id="2f376-123">String</span></span>                      | <span data-ttu-id="2f376-124">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="2f376-124">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="2f376-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2f376-125">resultInfo</span></span>                     | [<span data-ttu-id="2f376-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2f376-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="2f376-127">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="2f376-127">The result information.</span></span>  <span data-ttu-id="2f376-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f376-128">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2f376-129">status</span><span class="sxs-lookup"><span data-stu-id="2f376-129">status</span></span>                         | <span data-ttu-id="2f376-130">String</span><span class="sxs-lookup"><span data-stu-id="2f376-130">String</span></span>                      | <span data-ttu-id="2f376-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2f376-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="2f376-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f376-132">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="2f376-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f376-133">Relationships</span></span>
<span data-ttu-id="2f376-134">Нет</span><span class="sxs-lookup"><span data-stu-id="2f376-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f376-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f376-135">JSON representation</span></span>

<span data-ttu-id="2f376-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f376-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
