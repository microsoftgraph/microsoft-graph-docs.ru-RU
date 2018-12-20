---
title: Тип ресурса recordOperation
description: Тип recordOperation
author: VinodRavichandran
ms.openlocfilehash: 54b39f30df1dd53a95260b549ae9fab2eedddfd8
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380424"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="6a134-103">Тип ресурса recordOperation</span><span class="sxs-lookup"><span data-stu-id="6a134-103">recordOperation resource type</span></span>

> <span data-ttu-id="6a134-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6a134-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a134-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a134-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a134-106">Тип recordOperation</span><span class="sxs-lookup"><span data-stu-id="6a134-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="6a134-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a134-107">Properties</span></span>

| <span data-ttu-id="6a134-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a134-108">Property</span></span>                       | <span data-ttu-id="6a134-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a134-109">Type</span></span>                        | <span data-ttu-id="6a134-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a134-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6a134-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="6a134-111">clientContext</span></span>                  | <span data-ttu-id="6a134-112">String</span><span class="sxs-lookup"><span data-stu-id="6a134-112">String</span></span>                      | <span data-ttu-id="6a134-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="6a134-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="6a134-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="6a134-114">completionReason</span></span>               | <span data-ttu-id="6a134-115">String</span><span class="sxs-lookup"><span data-stu-id="6a134-115">String</span></span>                      | <span data-ttu-id="6a134-116">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="6a134-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="6a134-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a134-117">createdDateTime</span></span>                | <span data-ttu-id="6a134-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a134-118">DateTimeOffset</span></span>              | <span data-ttu-id="6a134-119">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="6a134-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="6a134-120">id</span><span class="sxs-lookup"><span data-stu-id="6a134-120">id</span></span>                             | <span data-ttu-id="6a134-121">String</span><span class="sxs-lookup"><span data-stu-id="6a134-121">String</span></span>                      | <span data-ttu-id="6a134-122">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a134-122">The server operation id. Read-only.</span></span> <span data-ttu-id="6a134-123">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="6a134-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="6a134-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6a134-124">lastActionDateTime</span></span>             | <span data-ttu-id="6a134-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a134-125">DateTimeOffset</span></span>              | <span data-ttu-id="6a134-126">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="6a134-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="6a134-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="6a134-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="6a134-128">String</span><span class="sxs-lookup"><span data-stu-id="6a134-128">String</span></span>                      | <span data-ttu-id="6a134-129">Маркер доступа, необходимые для извлечения записи.</span><span class="sxs-lookup"><span data-stu-id="6a134-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="6a134-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="6a134-130">recordResourceLocation</span></span>         | <span data-ttu-id="6a134-131">String</span><span class="sxs-lookup"><span data-stu-id="6a134-131">String</span></span>                      | <span data-ttu-id="6a134-132">Расположение, где расположена записи.</span><span class="sxs-lookup"><span data-stu-id="6a134-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="6a134-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a134-133">resultInfo</span></span>                     | [<span data-ttu-id="6a134-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a134-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="6a134-135">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="6a134-135">The result information.</span></span>  <span data-ttu-id="6a134-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a134-136">Read-only.</span></span> <span data-ttu-id="6a134-137">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="6a134-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="6a134-138">status</span><span class="sxs-lookup"><span data-stu-id="6a134-138">status</span></span>                         | <span data-ttu-id="6a134-139">String</span><span class="sxs-lookup"><span data-stu-id="6a134-139">String</span></span>                      | <span data-ttu-id="6a134-140">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6a134-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="6a134-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a134-141">Read-only.</span></span> <span data-ttu-id="6a134-142">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="6a134-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="6a134-143">Связи</span><span class="sxs-lookup"><span data-stu-id="6a134-143">Relationships</span></span>
<span data-ttu-id="6a134-144">Нет</span><span class="sxs-lookup"><span data-stu-id="6a134-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a134-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a134-145">JSON representation</span></span>

<span data-ttu-id="6a134-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a134-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="6a134-147">Пример</span><span class="sxs-lookup"><span data-stu-id="6a134-147">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
