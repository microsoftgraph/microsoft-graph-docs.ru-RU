---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3729078eb803cea09a998aee819904876e88c6c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508347"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="11f17-103">Тип ресурса Алерсистористате</span><span class="sxs-lookup"><span data-stu-id="11f17-103">alertHistoryState resource type</span></span>

<span data-ttu-id="11f17-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11f17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f17-105">Сохраняет изменения, внесенные в оповещения.</span><span class="sxs-lookup"><span data-stu-id="11f17-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="11f17-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11f17-106">Properties</span></span>

| <span data-ttu-id="11f17-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11f17-107">Property</span></span>     | <span data-ttu-id="11f17-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11f17-108">Type</span></span>        | <span data-ttu-id="11f17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11f17-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11f17-110">appId</span><span class="sxs-lookup"><span data-stu-id="11f17-110">appId</span></span>|<span data-ttu-id="11f17-111">String</span><span class="sxs-lookup"><span data-stu-id="11f17-111">String</span></span>| <span data-ttu-id="11f17-112">Идентификатор приложения для вызывающего приложения, отправившего обновление (исправление) в оповещение.</span><span class="sxs-lookup"><span data-stu-id="11f17-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="11f17-113">AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="11f17-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="11f17-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="11f17-114">assignedTo</span></span>|<span data-ttu-id="11f17-115">String</span><span class="sxs-lookup"><span data-stu-id="11f17-115">String</span></span>| <span data-ttu-id="11f17-116">UPN пользователя оповещение было назначено (Примечание: Alert. assignedTo содержит только Последнее значение/UPN).</span><span class="sxs-lookup"><span data-stu-id="11f17-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="11f17-117">comments</span><span class="sxs-lookup"><span data-stu-id="11f17-117">comments</span></span>|<span data-ttu-id="11f17-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="11f17-118">String collection</span></span>|<span data-ttu-id="11f17-119">Комментарий, введенный пользователем, который выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="11f17-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="11f17-120">feedback</span><span class="sxs-lookup"><span data-stu-id="11f17-120">feedback</span></span>|<span data-ttu-id="11f17-121">String</span><span class="sxs-lookup"><span data-stu-id="11f17-121">String</span></span>| <span data-ttu-id="11f17-122">Обратная связь аналитика с оповещением в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="11f17-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="11f17-123">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="11f17-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="11f17-124">status</span><span class="sxs-lookup"><span data-stu-id="11f17-124">status</span></span>|<span data-ttu-id="11f17-125">Строка</span><span class="sxs-lookup"><span data-stu-id="11f17-125">String</span></span>| <span data-ttu-id="11f17-126">Значение состояния оповещения (при обновлении).</span><span class="sxs-lookup"><span data-stu-id="11f17-126">Alert status value (if updated).</span></span> <span data-ttu-id="11f17-127">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="11f17-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="11f17-128">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="11f17-128">updatedDateTime</span></span>|<span data-ttu-id="11f17-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11f17-129">DateTimeOffset</span></span>| <span data-ttu-id="11f17-130">Дата и время обновления оповещения.</span><span class="sxs-lookup"><span data-stu-id="11f17-130">Date and time of the alert update.</span></span> <span data-ttu-id="11f17-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="11f17-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11f17-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11f17-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="11f17-133">user</span><span class="sxs-lookup"><span data-stu-id="11f17-133">user</span></span>|<span data-ttu-id="11f17-134">String</span><span class="sxs-lookup"><span data-stu-id="11f17-134">String</span></span>| <span data-ttu-id="11f17-135">UPN пользователя, выполнившего вход, который обновил оповещение (берется из маркера носителя — если в режиме пользователя или делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="11f17-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11f17-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11f17-136">JSON representation</span></span>

<span data-ttu-id="11f17-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11f17-137">The following is a JSON representation of the resource.</span></span>

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