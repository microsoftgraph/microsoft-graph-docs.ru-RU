---
title: Тип ресурса recordOperation
description: Тип recordOperation
ms.openlocfilehash: 5863e5ef84b00c65cd0806af8a3364fe3d1ab73f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076162"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="4ea25-103">Тип ресурса recordOperation</span><span class="sxs-lookup"><span data-stu-id="4ea25-103">recordOperation resource type</span></span>

> <span data-ttu-id="4ea25-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4ea25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ea25-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ea25-106">Тип recordOperation</span><span class="sxs-lookup"><span data-stu-id="4ea25-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="4ea25-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ea25-107">Properties</span></span>

| <span data-ttu-id="4ea25-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ea25-108">Property</span></span>                       | <span data-ttu-id="4ea25-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea25-109">Type</span></span>                        | <span data-ttu-id="4ea25-110">Description</span><span class="sxs-lookup"><span data-stu-id="4ea25-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4ea25-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="4ea25-111">clientContext</span></span>                  | <span data-ttu-id="4ea25-112">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-112">String</span></span>                      | <span data-ttu-id="4ea25-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="4ea25-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="4ea25-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="4ea25-114">completionReason</span></span>               | <span data-ttu-id="4ea25-115">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-115">String</span></span>                      | <span data-ttu-id="4ea25-116">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span><span class="sxs-lookup"><span data-stu-id="4ea25-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span></span> |
| <span data-ttu-id="4ea25-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea25-117">createdDateTime</span></span>                | <span data-ttu-id="4ea25-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea25-118">DateTimeOffset</span></span>              | <span data-ttu-id="4ea25-119">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="4ea25-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="4ea25-120">id</span><span class="sxs-lookup"><span data-stu-id="4ea25-120">id</span></span>                             | <span data-ttu-id="4ea25-121">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-121">String</span></span>                      | <span data-ttu-id="4ea25-122">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ea25-122">The server operation id. Read-only.</span></span> <span data-ttu-id="4ea25-123">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="4ea25-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4ea25-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea25-124">lastActionDateTime</span></span>             | <span data-ttu-id="4ea25-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea25-125">DateTimeOffset</span></span>              | <span data-ttu-id="4ea25-126">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="4ea25-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="4ea25-127">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="4ea25-127">recordResourceLocation</span></span>         | <span data-ttu-id="4ea25-128">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-128">String</span></span>                      | <span data-ttu-id="4ea25-129">Расположение, где расположена записи.</span><span class="sxs-lookup"><span data-stu-id="4ea25-129">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="4ea25-130">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="4ea25-130">recordResourceAccessToken</span></span>      | <span data-ttu-id="4ea25-131">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-131">String</span></span>                      | <span data-ttu-id="4ea25-132">Маркер доступа, необходимые для извлечения записи.</span><span class="sxs-lookup"><span data-stu-id="4ea25-132">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="4ea25-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4ea25-133">resultInfo</span></span>                     | [<span data-ttu-id="4ea25-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4ea25-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4ea25-135">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="4ea25-135">The result information.</span></span>  <span data-ttu-id="4ea25-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ea25-136">Read-only.</span></span> <span data-ttu-id="4ea25-137">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="4ea25-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4ea25-138">status</span><span class="sxs-lookup"><span data-stu-id="4ea25-138">status</span></span>                         | <span data-ttu-id="4ea25-139">String</span><span class="sxs-lookup"><span data-stu-id="4ea25-139">String</span></span>                      | <span data-ttu-id="4ea25-140">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4ea25-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4ea25-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ea25-141">Read-only.</span></span> <span data-ttu-id="4ea25-142">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="4ea25-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="4ea25-143">Связи</span><span class="sxs-lookup"><span data-stu-id="4ea25-143">Relationships</span></span>
<span data-ttu-id="4ea25-144">Нет</span><span class="sxs-lookup"><span data-stu-id="4ea25-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ea25-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ea25-145">JSON representation</span></span>

<span data-ttu-id="4ea25-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ea25-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceLocation": "String",
  "recordResourceAccessToken": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="4ea25-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4ea25-147">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
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
