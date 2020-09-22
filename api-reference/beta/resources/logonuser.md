---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 737a3ad71ee34641dd6d2c719a7a1975d3fb11ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075527"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="79f42-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="79f42-103">logonUser resource type</span></span>

<span data-ttu-id="79f42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f42-105">Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле</span><span class="sxs-lookup"><span data-stu-id="79f42-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="79f42-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="79f42-106">Properties</span></span>

| <span data-ttu-id="79f42-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="79f42-107">Property</span></span>   | <span data-ttu-id="79f42-108">Тип</span><span class="sxs-lookup"><span data-stu-id="79f42-108">Type</span></span> |<span data-ttu-id="79f42-109">Описание</span><span class="sxs-lookup"><span data-stu-id="79f42-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79f42-110">аккаунтдомаин</span><span class="sxs-lookup"><span data-stu-id="79f42-110">accountDomain</span></span>|<span data-ttu-id="79f42-111">String</span><span class="sxs-lookup"><span data-stu-id="79f42-111">String</span></span>|<span data-ttu-id="79f42-112">Домен учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="79f42-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="79f42-113">accountName</span><span class="sxs-lookup"><span data-stu-id="79f42-113">accountName</span></span>|<span data-ttu-id="79f42-114">String</span><span class="sxs-lookup"><span data-stu-id="79f42-114">String</span></span>|<span data-ttu-id="79f42-115">Имя учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="79f42-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="79f42-116">accountType</span><span class="sxs-lookup"><span data-stu-id="79f42-116">accountType</span></span>|<span data-ttu-id="79f42-117">String</span><span class="sxs-lookup"><span data-stu-id="79f42-117">String</span></span>|<span data-ttu-id="79f42-118">Тип учетной записи пользователя для каждого определения Windows.</span><span class="sxs-lookup"><span data-stu-id="79f42-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="79f42-119">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="79f42-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="79f42-120">фирстсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="79f42-120">firstSeenDateTime</span></span>|<span data-ttu-id="79f42-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f42-121">DateTimeOffset</span></span>|<span data-ttu-id="79f42-122">Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком).</span><span class="sxs-lookup"><span data-stu-id="79f42-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="79f42-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="79f42-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79f42-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="79f42-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="79f42-125">ластсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="79f42-125">lastSeenDateTime</span></span>|<span data-ttu-id="79f42-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f42-126">DateTimeOffset</span></span>|<span data-ttu-id="79f42-127">Дата и время последнего входа в систему с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="79f42-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="79f42-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="79f42-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79f42-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="79f42-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="79f42-130">логонид</span><span class="sxs-lookup"><span data-stu-id="79f42-130">logonId</span></span>|<span data-ttu-id="79f42-131">String</span><span class="sxs-lookup"><span data-stu-id="79f42-131">String</span></span>|<span data-ttu-id="79f42-132">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="79f42-132">User logon ID.</span></span>|
|<span data-ttu-id="79f42-133">Logontypes задано</span><span class="sxs-lookup"><span data-stu-id="79f42-133">logonTypes</span></span>|<span data-ttu-id="79f42-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79f42-134">String collection</span></span>|<span data-ttu-id="79f42-135">Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения.</span><span class="sxs-lookup"><span data-stu-id="79f42-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="79f42-136">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="79f42-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79f42-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79f42-137">JSON representation</span></span>

<span data-ttu-id="79f42-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79f42-138">The following is a JSON representation of the resource.</span></span>

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


