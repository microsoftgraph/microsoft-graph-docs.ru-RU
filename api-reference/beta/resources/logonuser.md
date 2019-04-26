---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562659"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="236d2-103">Тип ресурса logonUser</span><span class="sxs-lookup"><span data-stu-id="236d2-103">logonUser resource type</span></span>

<span data-ttu-id="236d2-104">Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле</span><span class="sxs-lookup"><span data-stu-id="236d2-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="236d2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="236d2-105">Properties</span></span>

| <span data-ttu-id="236d2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="236d2-106">Property</span></span>   | <span data-ttu-id="236d2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="236d2-107">Type</span></span> |<span data-ttu-id="236d2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="236d2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="236d2-109">Аккаунтдомаин</span><span class="sxs-lookup"><span data-stu-id="236d2-109">accountDomain</span></span>|<span data-ttu-id="236d2-110">String</span><span class="sxs-lookup"><span data-stu-id="236d2-110">String</span></span>|<span data-ttu-id="236d2-111">Домен учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="236d2-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="236d2-112">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="236d2-112">accountName</span></span>|<span data-ttu-id="236d2-113">String</span><span class="sxs-lookup"><span data-stu-id="236d2-113">String</span></span>|<span data-ttu-id="236d2-114">Имя учетной записи пользователя, используемой для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="236d2-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="236d2-115">accountType</span><span class="sxs-lookup"><span data-stu-id="236d2-115">accountType</span></span>|<span data-ttu-id="236d2-116">String</span><span class="sxs-lookup"><span data-stu-id="236d2-116">String</span></span>|<span data-ttu-id="236d2-117">Тип учетной записи пользователя для каждого определения Windows.</span><span class="sxs-lookup"><span data-stu-id="236d2-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="236d2-118">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="236d2-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="236d2-119">Фирстсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="236d2-119">firstSeenDateTime</span></span>|<span data-ttu-id="236d2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236d2-120">DateTimeOffset</span></span>|<span data-ttu-id="236d2-121">Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком).</span><span class="sxs-lookup"><span data-stu-id="236d2-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="236d2-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="236d2-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="236d2-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="236d2-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="236d2-124">Ластсиндатетиме</span><span class="sxs-lookup"><span data-stu-id="236d2-124">lastSeenDateTime</span></span>|<span data-ttu-id="236d2-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="236d2-125">DateTimeOffset</span></span>|<span data-ttu-id="236d2-126">Дата и время последнего входа в систему с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="236d2-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="236d2-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="236d2-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="236d2-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="236d2-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="236d2-129">Логонид</span><span class="sxs-lookup"><span data-stu-id="236d2-129">logonId</span></span>|<span data-ttu-id="236d2-130">String</span><span class="sxs-lookup"><span data-stu-id="236d2-130">String</span></span>|<span data-ttu-id="236d2-131">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="236d2-131">User logon ID.</span></span>|
|<span data-ttu-id="236d2-132">Logontypes задано</span><span class="sxs-lookup"><span data-stu-id="236d2-132">logonTypes</span></span>|<span data-ttu-id="236d2-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="236d2-133">String collection</span></span>|<span data-ttu-id="236d2-134">Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения.</span><span class="sxs-lookup"><span data-stu-id="236d2-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="236d2-135">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="236d2-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="236d2-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="236d2-136">JSON representation</span></span>

<span data-ttu-id="236d2-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="236d2-137">The following is a JSON representation of the resource.</span></span>

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
