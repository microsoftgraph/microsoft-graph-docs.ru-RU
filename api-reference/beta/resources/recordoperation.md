---
title: Тип ресурса Рекордоператион
description: Тип Рекордоператион
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00b05cd86eeb9cf8be26cdc09fb8a9b254b510db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008805"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="e7fd2-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="e7fd2-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fd2-104">Тип Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="e7fd2-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="e7fd2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7fd2-105">Properties</span></span>

| <span data-ttu-id="e7fd2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7fd2-106">Property</span></span>                       | <span data-ttu-id="e7fd2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e7fd2-107">Type</span></span>                        | <span data-ttu-id="e7fd2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e7fd2-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e7fd2-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="e7fd2-109">clientContext</span></span>                  | <span data-ttu-id="e7fd2-110">String</span><span class="sxs-lookup"><span data-stu-id="e7fd2-110">String</span></span>                      | <span data-ttu-id="e7fd2-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="e7fd2-112">Комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="e7fd2-112">completionReason</span></span>               | <span data-ttu-id="e7fd2-113">String</span><span class="sxs-lookup"><span data-stu-id="e7fd2-113">String</span></span>                      | <span data-ttu-id="e7fd2-114">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="e7fd2-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7fd2-115">createdDateTime</span></span>                | <span data-ttu-id="e7fd2-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7fd2-116">DateTimeOffset</span></span>              | <span data-ttu-id="e7fd2-117">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="e7fd2-118">id</span><span class="sxs-lookup"><span data-stu-id="e7fd2-118">id</span></span>                             | <span data-ttu-id="e7fd2-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e7fd2-119">String</span></span>                      | <span data-ttu-id="e7fd2-120">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-120">The server operation id. Read-only.</span></span> <span data-ttu-id="e7fd2-121">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e7fd2-122">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="e7fd2-122">lastActionDateTime</span></span>             | <span data-ttu-id="e7fd2-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7fd2-123">DateTimeOffset</span></span>              | <span data-ttu-id="e7fd2-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="e7fd2-125">Рекордресаурцеакцесстокен</span><span class="sxs-lookup"><span data-stu-id="e7fd2-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="e7fd2-126">String</span><span class="sxs-lookup"><span data-stu-id="e7fd2-126">String</span></span>                      | <span data-ttu-id="e7fd2-127">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="e7fd2-128">Рекордресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="e7fd2-128">recordResourceLocation</span></span>         | <span data-ttu-id="e7fd2-129">String</span><span class="sxs-lookup"><span data-stu-id="e7fd2-129">String</span></span>                      | <span data-ttu-id="e7fd2-130">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="e7fd2-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e7fd2-131">resultInfo</span></span>                     | [<span data-ttu-id="e7fd2-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e7fd2-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e7fd2-133">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-133">The result information.</span></span>  <span data-ttu-id="e7fd2-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-134">Read-only.</span></span> <span data-ttu-id="e7fd2-135">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e7fd2-136">status</span><span class="sxs-lookup"><span data-stu-id="e7fd2-136">status</span></span>                         | <span data-ttu-id="e7fd2-137">String</span><span class="sxs-lookup"><span data-stu-id="e7fd2-137">String</span></span>                      | <span data-ttu-id="e7fd2-138">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e7fd2-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-139">Read-only.</span></span> <span data-ttu-id="e7fd2-140">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="e7fd2-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="e7fd2-141">Relationships</span></span>
<span data-ttu-id="e7fd2-142">Нет</span><span class="sxs-lookup"><span data-stu-id="e7fd2-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7fd2-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7fd2-143">JSON representation</span></span>

<span data-ttu-id="e7fd2-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7fd2-144">The following is a JSON representation of the resource.</span></span>

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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="e7fd2-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e7fd2-145">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
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
