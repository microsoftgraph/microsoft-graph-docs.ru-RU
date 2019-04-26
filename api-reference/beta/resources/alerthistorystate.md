---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339158"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="18076-103">Тип ресурса Алерсистористате</span><span class="sxs-lookup"><span data-stu-id="18076-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18076-104">Сохраняет изменения, внесенные в оповещения.</span><span class="sxs-lookup"><span data-stu-id="18076-104">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="18076-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="18076-105">Properties</span></span>

| <span data-ttu-id="18076-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="18076-106">Property</span></span>     | <span data-ttu-id="18076-107">Тип</span><span class="sxs-lookup"><span data-stu-id="18076-107">Type</span></span>        | <span data-ttu-id="18076-108">Описание</span><span class="sxs-lookup"><span data-stu-id="18076-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18076-109">appId</span><span class="sxs-lookup"><span data-stu-id="18076-109">appId</span></span>|<span data-ttu-id="18076-110">String</span><span class="sxs-lookup"><span data-stu-id="18076-110">String</span></span>| <span data-ttu-id="18076-111">Идентификатор приложения для вызывающего приложения, отправившего обновление (исправление) в оповещение.</span><span class="sxs-lookup"><span data-stu-id="18076-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="18076-112">AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="18076-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="18076-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="18076-113">assignedTo</span></span>|<span data-ttu-id="18076-114">String</span><span class="sxs-lookup"><span data-stu-id="18076-114">String</span></span>| <span data-ttu-id="18076-115">UPN пользователя оповещение было назначено (Примечание: Alert. assignedTo содержит только Последнее значение/UPN).</span><span class="sxs-lookup"><span data-stu-id="18076-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="18076-116">comments</span><span class="sxs-lookup"><span data-stu-id="18076-116">comments</span></span>|<span data-ttu-id="18076-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18076-117">String collection</span></span>|<span data-ttu-id="18076-118">Комментарий, введенный пользователем, который выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="18076-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="18076-119">замечания</span><span class="sxs-lookup"><span data-stu-id="18076-119">feedback</span></span>|<span data-ttu-id="18076-120">String</span><span class="sxs-lookup"><span data-stu-id="18076-120">String</span></span>| <span data-ttu-id="18076-121">Обратная связь аналитика с оповещением в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="18076-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="18076-122">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="18076-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="18076-123">status</span><span class="sxs-lookup"><span data-stu-id="18076-123">status</span></span>|<span data-ttu-id="18076-124">Строка</span><span class="sxs-lookup"><span data-stu-id="18076-124">String</span></span>| <span data-ttu-id="18076-125">Значение состояния оповещения (при обновлении).</span><span class="sxs-lookup"><span data-stu-id="18076-125">Alert status value (if updated).</span></span> <span data-ttu-id="18076-126">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="18076-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="18076-127">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="18076-127">updatedDateTime</span></span>|<span data-ttu-id="18076-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18076-128">DateTimeOffset</span></span>| <span data-ttu-id="18076-129">Дата и время обновления оповещения.</span><span class="sxs-lookup"><span data-stu-id="18076-129">Date and time of the alert update.</span></span> <span data-ttu-id="18076-130">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="18076-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18076-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="18076-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="18076-132">user</span><span class="sxs-lookup"><span data-stu-id="18076-132">user</span></span>|<span data-ttu-id="18076-133">String</span><span class="sxs-lookup"><span data-stu-id="18076-133">String</span></span>| <span data-ttu-id="18076-134">UPN пользователя, выполнившего вход, который обновил оповещение (берется из маркера носителя — если в режиме пользователя или делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="18076-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18076-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18076-135">JSON representation</span></span>

<span data-ttu-id="18076-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18076-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->