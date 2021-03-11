---
title: тип ресурса logonUser
description: Содержит сведения о входе пользователя в этот хост
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9986aaa7cb5fbf5f8687c43de019b234a4a971d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720496"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="eff92-103">тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="eff92-103">logonUser resource type</span></span>

<span data-ttu-id="eff92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eff92-105">Содержит сведения о входе пользователя в этот хост</span><span class="sxs-lookup"><span data-stu-id="eff92-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="eff92-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="eff92-106">Properties</span></span>

| <span data-ttu-id="eff92-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="eff92-107">Property</span></span>   | <span data-ttu-id="eff92-108">Тип</span><span class="sxs-lookup"><span data-stu-id="eff92-108">Type</span></span> |<span data-ttu-id="eff92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eff92-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eff92-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="eff92-110">accountDomain</span></span>|<span data-ttu-id="eff92-111">String</span><span class="sxs-lookup"><span data-stu-id="eff92-111">String</span></span>|<span data-ttu-id="eff92-112">Домен учетной записи пользователя, используемый для логона.</span><span class="sxs-lookup"><span data-stu-id="eff92-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="eff92-113">accountName</span><span class="sxs-lookup"><span data-stu-id="eff92-113">accountName</span></span>|<span data-ttu-id="eff92-114">String</span><span class="sxs-lookup"><span data-stu-id="eff92-114">String</span></span>|<span data-ttu-id="eff92-115">Имя учетной записи учетной записи пользователя, используемой для логона.</span><span class="sxs-lookup"><span data-stu-id="eff92-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="eff92-116">accountType</span><span class="sxs-lookup"><span data-stu-id="eff92-116">accountType</span></span>|<span data-ttu-id="eff92-117">String</span><span class="sxs-lookup"><span data-stu-id="eff92-117">String</span></span>|<span data-ttu-id="eff92-118">Тип учетной записи пользователя по определению Windows.</span><span class="sxs-lookup"><span data-stu-id="eff92-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="eff92-119">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="eff92-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="eff92-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="eff92-120">firstSeenDateTime</span></span>|<span data-ttu-id="eff92-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eff92-121">DateTimeOffset</span></span>|<span data-ttu-id="eff92-122">DateTime, в котором произошел самый ранний логотип этой учетной записи пользователя (период, определяемый поставщиком).</span><span class="sxs-lookup"><span data-stu-id="eff92-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="eff92-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eff92-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eff92-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eff92-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="eff92-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="eff92-125">lastSeenDateTime</span></span>|<span data-ttu-id="eff92-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eff92-126">DateTimeOffset</span></span>|<span data-ttu-id="eff92-127">DateTime, в котором произошел последний логотип этой учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="eff92-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="eff92-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eff92-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eff92-129">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eff92-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="eff92-130">logonId</span><span class="sxs-lookup"><span data-stu-id="eff92-130">logonId</span></span>|<span data-ttu-id="eff92-131">String</span><span class="sxs-lookup"><span data-stu-id="eff92-131">String</span></span>|<span data-ttu-id="eff92-132">ID логотипа пользователя.</span><span class="sxs-lookup"><span data-stu-id="eff92-132">User logon ID.</span></span>|
|<span data-ttu-id="eff92-133">logonTypes</span><span class="sxs-lookup"><span data-stu-id="eff92-133">logonTypes</span></span>|<span data-ttu-id="eff92-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="eff92-134">String collection</span></span>|<span data-ttu-id="eff92-135">Коллекция типов логотипов, наблюдаемых для входа в систему пользователя с первого до последнего вида.</span><span class="sxs-lookup"><span data-stu-id="eff92-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="eff92-136">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="eff92-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eff92-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eff92-137">JSON representation</span></span>

<span data-ttu-id="eff92-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eff92-138">The following is a JSON representation of the resource.</span></span>

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


