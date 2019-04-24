---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461071"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="dd062-103">Тип ресурса Алерсистористате</span><span class="sxs-lookup"><span data-stu-id="dd062-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd062-104">Сохраняет изменения, внесенные в оповещения.</span><span class="sxs-lookup"><span data-stu-id="dd062-104">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="dd062-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd062-105">Properties</span></span>

| <span data-ttu-id="dd062-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd062-106">Property</span></span>     | <span data-ttu-id="dd062-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dd062-107">Type</span></span>        | <span data-ttu-id="dd062-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dd062-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd062-109">appId</span><span class="sxs-lookup"><span data-stu-id="dd062-109">appId</span></span>|<span data-ttu-id="dd062-110">String</span><span class="sxs-lookup"><span data-stu-id="dd062-110">String</span></span>| <span data-ttu-id="dd062-111">Идентификатор приложения для вызывающего приложения, отправившего обновление (исправление) в оповещение.</span><span class="sxs-lookup"><span data-stu-id="dd062-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="dd062-112">AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="dd062-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="dd062-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="dd062-113">assignedTo</span></span>|<span data-ttu-id="dd062-114">String</span><span class="sxs-lookup"><span data-stu-id="dd062-114">String</span></span>| <span data-ttu-id="dd062-115">UPN пользователя оповещение было назначено (Примечание: Alert. assignedTo содержит только Последнее значение/UPN).</span><span class="sxs-lookup"><span data-stu-id="dd062-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="dd062-116">comments</span><span class="sxs-lookup"><span data-stu-id="dd062-116">comments</span></span>|<span data-ttu-id="dd062-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dd062-117">String collection</span></span>|<span data-ttu-id="dd062-118">Комментарий, введенный пользователем, который выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="dd062-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="dd062-119">замечания</span><span class="sxs-lookup"><span data-stu-id="dd062-119">feedback</span></span>|<span data-ttu-id="dd062-120">String</span><span class="sxs-lookup"><span data-stu-id="dd062-120">String</span></span>| <span data-ttu-id="dd062-121">Обратная связь аналитика с оповещением в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="dd062-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="dd062-122">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="dd062-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="dd062-123">status</span><span class="sxs-lookup"><span data-stu-id="dd062-123">status</span></span>|<span data-ttu-id="dd062-124">Строка</span><span class="sxs-lookup"><span data-stu-id="dd062-124">String</span></span>| <span data-ttu-id="dd062-125">Значение состояния оповещения (при обновлении).</span><span class="sxs-lookup"><span data-stu-id="dd062-125">Alert status value (if updated).</span></span> <span data-ttu-id="dd062-126">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="dd062-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="dd062-127">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="dd062-127">updatedDateTime</span></span>|<span data-ttu-id="dd062-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd062-128">DateTimeOffset</span></span>| <span data-ttu-id="dd062-129">Дата и время обновления оповещения.</span><span class="sxs-lookup"><span data-stu-id="dd062-129">Date and time of the alert update.</span></span> <span data-ttu-id="dd062-130">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="dd062-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd062-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="dd062-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dd062-132">user</span><span class="sxs-lookup"><span data-stu-id="dd062-132">user</span></span>|<span data-ttu-id="dd062-133">String</span><span class="sxs-lookup"><span data-stu-id="dd062-133">String</span></span>| <span data-ttu-id="dd062-134">UPN пользователя, выполнившего вход, который обновил оповещение (берется из маркера носителя — если в режиме пользователя или делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="dd062-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd062-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd062-135">JSON representation</span></span>

<span data-ttu-id="dd062-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd062-136">The following is a JSON representation of the resource.</span></span>

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