---
title: тип ресурса alertHistoryState
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2bc1c1a58f6f7f073b6803adbee07b4b2990a0e1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722169"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="00c25-103">тип ресурса alertHistoryState</span><span class="sxs-lookup"><span data-stu-id="00c25-103">alertHistoryState resource type</span></span>

<span data-ttu-id="00c25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00c25-105">Сохраняет изменения, внесенные в оповещения.</span><span class="sxs-lookup"><span data-stu-id="00c25-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="00c25-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="00c25-106">Properties</span></span>

| <span data-ttu-id="00c25-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="00c25-107">Property</span></span>     | <span data-ttu-id="00c25-108">Тип</span><span class="sxs-lookup"><span data-stu-id="00c25-108">Type</span></span>        | <span data-ttu-id="00c25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00c25-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00c25-110">appId</span><span class="sxs-lookup"><span data-stu-id="00c25-110">appId</span></span>|<span data-ttu-id="00c25-111">String</span><span class="sxs-lookup"><span data-stu-id="00c25-111">String</span></span>| <span data-ttu-id="00c25-112">ID приложения вызываемого приложения, которое отправило обновление (PATCH) в оповещение.</span><span class="sxs-lookup"><span data-stu-id="00c25-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="00c25-113">AppId должен быть извлечен из маркера auth и не вошел вручную в вызываемом приложении.</span><span class="sxs-lookup"><span data-stu-id="00c25-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="00c25-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="00c25-114">assignedTo</span></span>|<span data-ttu-id="00c25-115">String</span><span class="sxs-lookup"><span data-stu-id="00c25-115">String</span></span>| <span data-ttu-id="00c25-116">UPN пользователя оповещение было назначено (примечание: alert.assignedTo сохраняет только последнее значение/UPN).</span><span class="sxs-lookup"><span data-stu-id="00c25-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="00c25-117">comments</span><span class="sxs-lookup"><span data-stu-id="00c25-117">comments</span></span>|<span data-ttu-id="00c25-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="00c25-118">String collection</span></span>|<span data-ttu-id="00c25-119">Комментарий, вписаный пользователем с входом.</span><span class="sxs-lookup"><span data-stu-id="00c25-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="00c25-120">feedback</span><span class="sxs-lookup"><span data-stu-id="00c25-120">feedback</span></span>|<span data-ttu-id="00c25-121">String</span><span class="sxs-lookup"><span data-stu-id="00c25-121">String</span></span>| <span data-ttu-id="00c25-122">Отзывы аналитика об оповещении в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="00c25-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="00c25-123">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="00c25-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="00c25-124">status</span><span class="sxs-lookup"><span data-stu-id="00c25-124">status</span></span>|<span data-ttu-id="00c25-125">String</span><span class="sxs-lookup"><span data-stu-id="00c25-125">String</span></span>| <span data-ttu-id="00c25-126">Значение состояния оповещений (если обновлено).</span><span class="sxs-lookup"><span data-stu-id="00c25-126">Alert status value (if updated).</span></span> <span data-ttu-id="00c25-127">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="00c25-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="00c25-128">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="00c25-128">updatedDateTime</span></span>|<span data-ttu-id="00c25-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00c25-129">DateTimeOffset</span></span>| <span data-ttu-id="00c25-130">Дата и время обновления оповещений.</span><span class="sxs-lookup"><span data-stu-id="00c25-130">Date and time of the alert update.</span></span> <span data-ttu-id="00c25-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="00c25-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00c25-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="00c25-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="00c25-133">user</span><span class="sxs-lookup"><span data-stu-id="00c25-133">user</span></span>|<span data-ttu-id="00c25-134">String</span><span class="sxs-lookup"><span data-stu-id="00c25-134">String</span></span>| <span data-ttu-id="00c25-135">UPN пользователя, который обновил оповещение (взято из маркера носитела — если в режиме пользовательского/делегирования auth).</span><span class="sxs-lookup"><span data-stu-id="00c25-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00c25-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00c25-136">JSON representation</span></span>

<span data-ttu-id="00c25-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00c25-137">The following is a JSON representation of the resource.</span></span>

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

