---
title: Тип ресурса Рекордоператион
description: Тип Рекордоператион
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 75760e38dde13a02624db987d521e3b02977901d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343933"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="b4477-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="b4477-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4477-104">Тип Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="b4477-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="b4477-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4477-105">Properties</span></span>

| <span data-ttu-id="b4477-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4477-106">Property</span></span>                       | <span data-ttu-id="b4477-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b4477-107">Type</span></span>                        | <span data-ttu-id="b4477-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b4477-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b4477-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="b4477-109">clientContext</span></span>                  | <span data-ttu-id="b4477-110">String</span><span class="sxs-lookup"><span data-stu-id="b4477-110">String</span></span>                      | <span data-ttu-id="b4477-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b4477-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="b4477-112">Комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="b4477-112">completionReason</span></span>               | <span data-ttu-id="b4477-113">String</span><span class="sxs-lookup"><span data-stu-id="b4477-113">String</span></span>                      | <span data-ttu-id="b4477-114">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b4477-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="b4477-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4477-115">createdDateTime</span></span>                | <span data-ttu-id="b4477-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4477-116">DateTimeOffset</span></span>              | <span data-ttu-id="b4477-117">Время создания записи.</span><span class="sxs-lookup"><span data-stu-id="b4477-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="b4477-118">id</span><span class="sxs-lookup"><span data-stu-id="b4477-118">id</span></span>                             | <span data-ttu-id="b4477-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b4477-119">String</span></span>                      | <span data-ttu-id="b4477-120">Идентификатор операции сервера. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4477-120">The server operation id. Read-only.</span></span> <span data-ttu-id="b4477-121">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="b4477-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="b4477-122">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b4477-122">lastActionDateTime</span></span>             | <span data-ttu-id="b4477-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4477-123">DateTimeOffset</span></span>              | <span data-ttu-id="b4477-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="b4477-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="b4477-125">Рекордресаурцеакцесстокен</span><span class="sxs-lookup"><span data-stu-id="b4477-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="b4477-126">String</span><span class="sxs-lookup"><span data-stu-id="b4477-126">String</span></span>                      | <span data-ttu-id="b4477-127">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="b4477-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="b4477-128">Рекордресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="b4477-128">recordResourceLocation</span></span>         | <span data-ttu-id="b4477-129">String</span><span class="sxs-lookup"><span data-stu-id="b4477-129">String</span></span>                      | <span data-ttu-id="b4477-130">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="b4477-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="b4477-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b4477-131">resultInfo</span></span>                     | [<span data-ttu-id="b4477-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b4477-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b4477-133">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="b4477-133">The result information.</span></span>  <span data-ttu-id="b4477-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4477-134">Read-only.</span></span> <span data-ttu-id="b4477-135">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="b4477-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="b4477-136">status</span><span class="sxs-lookup"><span data-stu-id="b4477-136">status</span></span>                         | <span data-ttu-id="b4477-137">String</span><span class="sxs-lookup"><span data-stu-id="b4477-137">String</span></span>                      | <span data-ttu-id="b4477-138">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b4477-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b4477-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4477-139">Read-only.</span></span> <span data-ttu-id="b4477-140">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="b4477-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="b4477-141">Связи</span><span class="sxs-lookup"><span data-stu-id="b4477-141">Relationships</span></span>
<span data-ttu-id="b4477-142">Нет</span><span class="sxs-lookup"><span data-stu-id="b4477-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4477-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4477-143">JSON representation</span></span>

<span data-ttu-id="b4477-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4477-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b4477-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b4477-145">Example</span></span>

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
