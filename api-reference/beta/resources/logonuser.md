---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 08053b2e3ba42c167edebb3678b41ccb3531e078
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009918"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="0cd22-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="0cd22-103">logonUser resource type</span></span>

<span data-ttu-id="0cd22-104">Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле</span><span class="sxs-lookup"><span data-stu-id="0cd22-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="0cd22-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cd22-105">Properties</span></span>

| <span data-ttu-id="0cd22-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd22-106">Property</span></span>   | <span data-ttu-id="0cd22-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0cd22-107">Type</span></span> |<span data-ttu-id="0cd22-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd22-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cd22-109">Аккаунтдомаин</span><span class="sxs-lookup"><span data-stu-id="0cd22-109">accountDomain</span></span>|<span data-ttu-id="0cd22-110">String</span><span class="sxs-lookup"><span data-stu-id="0cd22-110">String</span></span>|<span data-ttu-id="0cd22-111">Домен учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="0cd22-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="0cd22-112">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="0cd22-112">accountName</span></span>|<span data-ttu-id="0cd22-113">String</span><span class="sxs-lookup"><span data-stu-id="0cd22-113">String</span></span>|<span data-ttu-id="0cd22-114">Имя учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="0cd22-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="0cd22-115">accountType</span><span class="sxs-lookup"><span data-stu-id="0cd22-115">accountType</span></span>|<span data-ttu-id="0cd22-116">String</span><span class="sxs-lookup"><span data-stu-id="0cd22-116">String</span></span>|<span data-ttu-id="0cd22-117">Тип учетной записи пользователя для каждого определения Windows.</span><span class="sxs-lookup"><span data-stu-id="0cd22-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="0cd22-118">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="0cd22-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="0cd22-119">Фирстсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="0cd22-119">firstSeenDateTime</span></span>|<span data-ttu-id="0cd22-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd22-120">DateTimeOffset</span></span>|<span data-ttu-id="0cd22-121">Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком).</span><span class="sxs-lookup"><span data-stu-id="0cd22-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="0cd22-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0cd22-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0cd22-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0cd22-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0cd22-124">Ластсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="0cd22-124">lastSeenDateTime</span></span>|<span data-ttu-id="0cd22-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd22-125">DateTimeOffset</span></span>|<span data-ttu-id="0cd22-126">Дата и время последнего входа в систему с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cd22-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="0cd22-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0cd22-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0cd22-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0cd22-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0cd22-129">Логонид</span><span class="sxs-lookup"><span data-stu-id="0cd22-129">logonId</span></span>|<span data-ttu-id="0cd22-130">String</span><span class="sxs-lookup"><span data-stu-id="0cd22-130">String</span></span>|<span data-ttu-id="0cd22-131">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cd22-131">User logon ID.</span></span>|
|<span data-ttu-id="0cd22-132">Logontypes задано</span><span class="sxs-lookup"><span data-stu-id="0cd22-132">logonTypes</span></span>|<span data-ttu-id="0cd22-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0cd22-133">String collection</span></span>|<span data-ttu-id="0cd22-134">Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения.</span><span class="sxs-lookup"><span data-stu-id="0cd22-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="0cd22-135">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="0cd22-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cd22-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cd22-136">JSON representation</span></span>

<span data-ttu-id="0cd22-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cd22-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
