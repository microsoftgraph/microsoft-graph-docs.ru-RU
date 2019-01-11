---
title: Тип ресурса logonUser
description: Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855596"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="414ce-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="414ce-103">logonUser resource type</span></span>

<span data-ttu-id="414ce-104">Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле</span><span class="sxs-lookup"><span data-stu-id="414ce-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="414ce-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="414ce-105">Properties</span></span>

| <span data-ttu-id="414ce-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="414ce-106">Property</span></span>   | <span data-ttu-id="414ce-107">Тип</span><span class="sxs-lookup"><span data-stu-id="414ce-107">Type</span></span> |<span data-ttu-id="414ce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="414ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="414ce-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="414ce-109">accountDomain</span></span>|<span data-ttu-id="414ce-110">Строка</span><span class="sxs-lookup"><span data-stu-id="414ce-110">String</span></span>|<span data-ttu-id="414ce-111">Домен учетной записи пользователя, используемое для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="414ce-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="414ce-112">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="414ce-112">accountName</span></span>|<span data-ttu-id="414ce-113">Строка</span><span class="sxs-lookup"><span data-stu-id="414ce-113">String</span></span>|<span data-ttu-id="414ce-114">Имя учетной записи учетная запись пользователя, используемая для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="414ce-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="414ce-115">accountType</span><span class="sxs-lookup"><span data-stu-id="414ce-115">accountType</span></span>|<span data-ttu-id="414ce-116">Строка</span><span class="sxs-lookup"><span data-stu-id="414ce-116">String</span></span>|<span data-ttu-id="414ce-117">Тип учетной записи пользователя, для определения Windows.</span><span class="sxs-lookup"><span data-stu-id="414ce-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="414ce-118">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="414ce-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="414ce-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="414ce-119">firstSeenDateTime</span></span>|<span data-ttu-id="414ce-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="414ce-120">DateTimeOffset</span></span>|<span data-ttu-id="414ce-121">DateTime, в которой произошло раннюю вход в систему с этой учетной записи пользователя (определяются поставщика период).</span><span class="sxs-lookup"><span data-stu-id="414ce-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="414ce-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="414ce-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="414ce-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="414ce-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="414ce-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="414ce-124">lastSeenDateTime</span></span>|<span data-ttu-id="414ce-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="414ce-125">DateTimeOffset</span></span>|<span data-ttu-id="414ce-126">DateTime, в которой произошло последнего входа в систему с этой учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="414ce-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="414ce-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="414ce-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="414ce-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="414ce-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="414ce-129">logonId</span><span class="sxs-lookup"><span data-stu-id="414ce-129">logonId</span></span>|<span data-ttu-id="414ce-130">Строка</span><span class="sxs-lookup"><span data-stu-id="414ce-130">String</span></span>|<span data-ttu-id="414ce-131">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="414ce-131">User logon ID.</span></span>|
|<span data-ttu-id="414ce-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="414ce-132">logonTypes</span></span>|<span data-ttu-id="414ce-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="414ce-133">String collection</span></span>|<span data-ttu-id="414ce-134">Коллекция типов входа в систему, наблюдаемая для пользователя, выполнившего вход из при до последнего Заметим.</span><span class="sxs-lookup"><span data-stu-id="414ce-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="414ce-135">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="414ce-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="414ce-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="414ce-136">JSON representation</span></span>

<span data-ttu-id="414ce-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="414ce-137">The following is a JSON representation of the resource.</span></span>

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
