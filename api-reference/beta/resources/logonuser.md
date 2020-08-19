---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f480ff8c67c602512d7d8ef3f090366734f0ca7e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808664"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="e9760-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="e9760-103">logonUser resource type</span></span>

<span data-ttu-id="e9760-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9760-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9760-105">Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле</span><span class="sxs-lookup"><span data-stu-id="e9760-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="e9760-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9760-106">Properties</span></span>

| <span data-ttu-id="e9760-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9760-107">Property</span></span>   | <span data-ttu-id="e9760-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9760-108">Type</span></span> |<span data-ttu-id="e9760-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9760-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9760-110">аккаунтдомаин</span><span class="sxs-lookup"><span data-stu-id="e9760-110">accountDomain</span></span>|<span data-ttu-id="e9760-111">String</span><span class="sxs-lookup"><span data-stu-id="e9760-111">String</span></span>|<span data-ttu-id="e9760-112">Домен учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="e9760-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="e9760-113">accountName</span><span class="sxs-lookup"><span data-stu-id="e9760-113">accountName</span></span>|<span data-ttu-id="e9760-114">String</span><span class="sxs-lookup"><span data-stu-id="e9760-114">String</span></span>|<span data-ttu-id="e9760-115">Имя учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="e9760-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="e9760-116">accountType</span><span class="sxs-lookup"><span data-stu-id="e9760-116">accountType</span></span>|<span data-ttu-id="e9760-117">String</span><span class="sxs-lookup"><span data-stu-id="e9760-117">String</span></span>|<span data-ttu-id="e9760-118">Тип учетной записи пользователя для каждого определения Windows.</span><span class="sxs-lookup"><span data-stu-id="e9760-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="e9760-119">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e9760-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e9760-120">фирстсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="e9760-120">firstSeenDateTime</span></span>|<span data-ttu-id="e9760-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9760-121">DateTimeOffset</span></span>|<span data-ttu-id="e9760-122">Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком).</span><span class="sxs-lookup"><span data-stu-id="e9760-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="e9760-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9760-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9760-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9760-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e9760-125">ластсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="e9760-125">lastSeenDateTime</span></span>|<span data-ttu-id="e9760-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9760-126">DateTimeOffset</span></span>|<span data-ttu-id="e9760-127">Дата и время последнего входа в систему с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9760-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="e9760-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9760-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9760-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9760-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e9760-130">логонид</span><span class="sxs-lookup"><span data-stu-id="e9760-130">logonId</span></span>|<span data-ttu-id="e9760-131">String</span><span class="sxs-lookup"><span data-stu-id="e9760-131">String</span></span>|<span data-ttu-id="e9760-132">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9760-132">User logon ID.</span></span>|
|<span data-ttu-id="e9760-133">Logontypes задано</span><span class="sxs-lookup"><span data-stu-id="e9760-133">logonTypes</span></span>|<span data-ttu-id="e9760-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e9760-134">String collection</span></span>|<span data-ttu-id="e9760-135">Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e9760-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="e9760-136">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="e9760-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9760-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e9760-137">JSON representation</span></span>

<span data-ttu-id="e9760-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9760-138">The following is a JSON representation of the resource.</span></span>

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
