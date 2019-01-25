---
title: Тип ресурса recordOperation
description: Тип recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512509"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="af731-103">Тип ресурса recordOperation</span><span class="sxs-lookup"><span data-stu-id="af731-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af731-104">Тип recordOperation</span><span class="sxs-lookup"><span data-stu-id="af731-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="af731-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="af731-105">Properties</span></span>

| <span data-ttu-id="af731-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="af731-106">Property</span></span>                       | <span data-ttu-id="af731-107">Тип</span><span class="sxs-lookup"><span data-stu-id="af731-107">Type</span></span>                        | <span data-ttu-id="af731-108">Описание</span><span class="sxs-lookup"><span data-stu-id="af731-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="af731-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="af731-109">clientContext</span></span>                  | <span data-ttu-id="af731-110">String</span><span class="sxs-lookup"><span data-stu-id="af731-110">String</span></span>                      | <span data-ttu-id="af731-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="af731-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="af731-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="af731-112">completionReason</span></span>               | <span data-ttu-id="af731-113">String</span><span class="sxs-lookup"><span data-stu-id="af731-113">String</span></span>                      | <span data-ttu-id="af731-114">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="af731-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="af731-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af731-115">createdDateTime</span></span>                | <span data-ttu-id="af731-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af731-116">DateTimeOffset</span></span>              | <span data-ttu-id="af731-117">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="af731-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="af731-118">id</span><span class="sxs-lookup"><span data-stu-id="af731-118">id</span></span>                             | <span data-ttu-id="af731-119">String</span><span class="sxs-lookup"><span data-stu-id="af731-119">String</span></span>                      | <span data-ttu-id="af731-120">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af731-120">The server operation id. Read-only.</span></span> <span data-ttu-id="af731-121">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="af731-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="af731-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="af731-122">lastActionDateTime</span></span>             | <span data-ttu-id="af731-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af731-123">DateTimeOffset</span></span>              | <span data-ttu-id="af731-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="af731-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="af731-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="af731-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="af731-126">String</span><span class="sxs-lookup"><span data-stu-id="af731-126">String</span></span>                      | <span data-ttu-id="af731-127">Маркер доступа, необходимые для извлечения записи.</span><span class="sxs-lookup"><span data-stu-id="af731-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="af731-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="af731-128">recordResourceLocation</span></span>         | <span data-ttu-id="af731-129">String</span><span class="sxs-lookup"><span data-stu-id="af731-129">String</span></span>                      | <span data-ttu-id="af731-130">Расположение, где расположена записи.</span><span class="sxs-lookup"><span data-stu-id="af731-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="af731-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="af731-131">resultInfo</span></span>                     | [<span data-ttu-id="af731-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="af731-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="af731-133">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="af731-133">The result information.</span></span>  <span data-ttu-id="af731-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af731-134">Read-only.</span></span> <span data-ttu-id="af731-135">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="af731-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="af731-136">status</span><span class="sxs-lookup"><span data-stu-id="af731-136">status</span></span>                         | <span data-ttu-id="af731-137">String</span><span class="sxs-lookup"><span data-stu-id="af731-137">String</span></span>                      | <span data-ttu-id="af731-138">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="af731-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="af731-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af731-139">Read-only.</span></span> <span data-ttu-id="af731-140">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="af731-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="af731-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="af731-141">Relationships</span></span>
<span data-ttu-id="af731-142">Нет</span><span class="sxs-lookup"><span data-stu-id="af731-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af731-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af731-143">JSON representation</span></span>

<span data-ttu-id="af731-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af731-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="af731-145">Пример</span><span class="sxs-lookup"><span data-stu-id="af731-145">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
