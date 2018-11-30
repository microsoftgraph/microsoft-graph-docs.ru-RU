---
title: Тип ресурса logonUser
description: Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле
ms.openlocfilehash: 80ff69453e99f5cd5103f85cd7d8c45696057f7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081792"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="6391f-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="6391f-103">logonUser resource type</span></span>

<span data-ttu-id="6391f-104">Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле</span><span class="sxs-lookup"><span data-stu-id="6391f-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="6391f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6391f-105">Properties</span></span>

| <span data-ttu-id="6391f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6391f-106">Property</span></span>   | <span data-ttu-id="6391f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6391f-107">Type</span></span> |<span data-ttu-id="6391f-108">Description</span><span class="sxs-lookup"><span data-stu-id="6391f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6391f-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="6391f-109">accountDomain</span></span>|<span data-ttu-id="6391f-110">String</span><span class="sxs-lookup"><span data-stu-id="6391f-110">String</span></span>|<span data-ttu-id="6391f-111">Домен учетной записи пользователя, используемое для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="6391f-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="6391f-112">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="6391f-112">accountName</span></span>|<span data-ttu-id="6391f-113">String</span><span class="sxs-lookup"><span data-stu-id="6391f-113">String</span></span>|<span data-ttu-id="6391f-114">Имя учетной записи учетная запись пользователя, используемая для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="6391f-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="6391f-115">accountType</span><span class="sxs-lookup"><span data-stu-id="6391f-115">accountType</span></span>|<span data-ttu-id="6391f-116">String</span><span class="sxs-lookup"><span data-stu-id="6391f-116">String</span></span>|<span data-ttu-id="6391f-117">Тип учетной записи пользователя, для определения Windows.</span><span class="sxs-lookup"><span data-stu-id="6391f-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="6391f-118">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="6391f-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="6391f-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="6391f-119">firstSeenDateTime</span></span>|<span data-ttu-id="6391f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6391f-120">DateTimeOffset</span></span>|<span data-ttu-id="6391f-121">DateTime, в которой произошло раннюю вход в систему с этой учетной записи пользователя (определяются поставщика период).</span><span class="sxs-lookup"><span data-stu-id="6391f-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="6391f-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6391f-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6391f-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6391f-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6391f-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="6391f-124">lastSeenDateTime</span></span>|<span data-ttu-id="6391f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6391f-125">DateTimeOffset</span></span>|<span data-ttu-id="6391f-126">DateTime, в которой произошло последнего входа в систему с этой учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="6391f-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="6391f-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6391f-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6391f-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6391f-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6391f-129">logonId</span><span class="sxs-lookup"><span data-stu-id="6391f-129">logonId</span></span>|<span data-ttu-id="6391f-130">String</span><span class="sxs-lookup"><span data-stu-id="6391f-130">String</span></span>|<span data-ttu-id="6391f-131">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="6391f-131">User logon ID.</span></span>|
|<span data-ttu-id="6391f-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="6391f-132">logonTypes</span></span>|<span data-ttu-id="6391f-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6391f-133">String collection</span></span>|<span data-ttu-id="6391f-134">Коллекция типов входа в систему, наблюдаемая для пользователя, выполнившего вход из при до последнего Заметим.</span><span class="sxs-lookup"><span data-stu-id="6391f-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="6391f-135">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="6391f-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6391f-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6391f-136">JSON representation</span></span>

<span data-ttu-id="6391f-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6391f-137">The following is a JSON representation of the resource.</span></span>

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