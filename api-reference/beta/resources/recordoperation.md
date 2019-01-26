---
title: Тип ресурса recordOperation
description: Тип recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 914b8d819fdbcc132d4e04cd12f5c0db9980f659
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577188"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="5091e-103">Тип ресурса recordOperation</span><span class="sxs-lookup"><span data-stu-id="5091e-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5091e-104">Тип recordOperation</span><span class="sxs-lookup"><span data-stu-id="5091e-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="5091e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5091e-105">Properties</span></span>

| <span data-ttu-id="5091e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5091e-106">Property</span></span>                       | <span data-ttu-id="5091e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5091e-107">Type</span></span>                        | <span data-ttu-id="5091e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5091e-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5091e-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="5091e-109">clientContext</span></span>                  | <span data-ttu-id="5091e-110">Строка</span><span class="sxs-lookup"><span data-stu-id="5091e-110">String</span></span>                      | <span data-ttu-id="5091e-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="5091e-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="5091e-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="5091e-112">completionReason</span></span>               | <span data-ttu-id="5091e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5091e-113">String</span></span>                      | <span data-ttu-id="5091e-114">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="5091e-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="5091e-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5091e-115">createdDateTime</span></span>                | <span data-ttu-id="5091e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5091e-116">DateTimeOffset</span></span>              | <span data-ttu-id="5091e-117">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="5091e-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="5091e-118">id</span><span class="sxs-lookup"><span data-stu-id="5091e-118">id</span></span>                             | <span data-ttu-id="5091e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="5091e-119">String</span></span>                      | <span data-ttu-id="5091e-120">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5091e-120">The server operation id. Read-only.</span></span> <span data-ttu-id="5091e-121">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="5091e-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="5091e-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5091e-122">lastActionDateTime</span></span>             | <span data-ttu-id="5091e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5091e-123">DateTimeOffset</span></span>              | <span data-ttu-id="5091e-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="5091e-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="5091e-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="5091e-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="5091e-126">Строка</span><span class="sxs-lookup"><span data-stu-id="5091e-126">String</span></span>                      | <span data-ttu-id="5091e-127">Маркер доступа, необходимые для извлечения записи.</span><span class="sxs-lookup"><span data-stu-id="5091e-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="5091e-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="5091e-128">recordResourceLocation</span></span>         | <span data-ttu-id="5091e-129">Строка</span><span class="sxs-lookup"><span data-stu-id="5091e-129">String</span></span>                      | <span data-ttu-id="5091e-130">Расположение, где расположена записи.</span><span class="sxs-lookup"><span data-stu-id="5091e-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="5091e-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5091e-131">resultInfo</span></span>                     | [<span data-ttu-id="5091e-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5091e-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="5091e-133">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="5091e-133">The result information.</span></span>  <span data-ttu-id="5091e-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5091e-134">Read-only.</span></span> <span data-ttu-id="5091e-135">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="5091e-135">Server generated.</span></span>                                                                                             |

## <a name="relationships"></a><span data-ttu-id="5091e-136">Связи</span><span class="sxs-lookup"><span data-stu-id="5091e-136">Relationships</span></span>
<span data-ttu-id="5091e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5091e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5091e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5091e-138">JSON representation</span></span>

<span data-ttu-id="5091e-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5091e-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "recordCompletionReason",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"}
}
```

## <a name="example"></a><span data-ttu-id="5091e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5091e-140">Example</span></span>

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
