---
title: Тип ресурса "процесс"
description: Содержит сведения о состоянии процесса, связанного с оповещением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ccaf2e3048fc26573e9599a515aabf391dda6d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035086"
---
# <a name="process-resource-type"></a><span data-ttu-id="453eb-103">Тип ресурса "процесс"</span><span class="sxs-lookup"><span data-stu-id="453eb-103">process resource type</span></span>

<span data-ttu-id="453eb-104">Содержит сведения о состоянии процесса, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="453eb-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="453eb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="453eb-105">Properties</span></span>

| <span data-ttu-id="453eb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="453eb-106">Property</span></span>   | <span data-ttu-id="453eb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="453eb-107">Type</span></span>|<span data-ttu-id="453eb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="453eb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="453eb-109">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="453eb-109">accountName</span></span>|<span data-ttu-id="453eb-110">String</span><span class="sxs-lookup"><span data-stu-id="453eb-110">String</span></span>|<span data-ttu-id="453eb-111">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, который выполнялся в данный процесс) например, имя_учетной_записи, SID и т. д.</span><span class="sxs-lookup"><span data-stu-id="453eb-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="453eb-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="453eb-112">commandLine</span></span>|<span data-ttu-id="453eb-113">String</span><span class="sxs-lookup"><span data-stu-id="453eb-113">String</span></span>|<span data-ttu-id="453eb-114">Командная строка вызова полной обработки, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="453eb-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="453eb-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="453eb-115">createdDateTime</span></span>|<span data-ttu-id="453eb-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453eb-116">DateTimeOffset</span></span>|<span data-ttu-id="453eb-117">Время запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-117">Time at which the process was started.</span></span> <span data-ttu-id="453eb-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="453eb-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="453eb-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="453eb-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="453eb-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="453eb-120">fileHash</span></span>|[<span data-ttu-id="453eb-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="453eb-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="453eb-122">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="453eb-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="453eb-123">Интегритилевел</span><span class="sxs-lookup"><span data-stu-id="453eb-123">integrityLevel</span></span>|<span data-ttu-id="453eb-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="453eb-124">processIntegrityLevel</span></span>|<span data-ttu-id="453eb-125">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-125">The integrity level of the process.</span></span> <span data-ttu-id="453eb-126">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="453eb-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="453eb-127">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="453eb-127">isElevated</span></span>|<span data-ttu-id="453eb-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="453eb-128">Boolean</span></span>|<span data-ttu-id="453eb-129">Значение true, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="453eb-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="453eb-130">name</span><span class="sxs-lookup"><span data-stu-id="453eb-130">name</span></span>|<span data-ttu-id="453eb-131">String</span><span class="sxs-lookup"><span data-stu-id="453eb-131">String</span></span>|<span data-ttu-id="453eb-132">Имя файла образа процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="453eb-133">Парентпроцесскреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="453eb-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="453eb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453eb-134">DateTimeOffset</span></span>|<span data-ttu-id="453eb-135">Дата и время начала родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="453eb-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="453eb-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="453eb-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="453eb-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="453eb-138">Парентпроцессид</span><span class="sxs-lookup"><span data-stu-id="453eb-138">parentProcessId</span></span>|<span data-ttu-id="453eb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="453eb-139">Int32</span></span>|<span data-ttu-id="453eb-140">Идентификатор процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="453eb-141">Парентпроцесснаме</span><span class="sxs-lookup"><span data-stu-id="453eb-141">parentProcessName</span></span>|<span data-ttu-id="453eb-142">String</span><span class="sxs-lookup"><span data-stu-id="453eb-142">String</span></span>|<span data-ttu-id="453eb-143">Имя файла образа родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="453eb-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="453eb-144">path</span><span class="sxs-lookup"><span data-stu-id="453eb-144">path</span></span>|<span data-ttu-id="453eb-145">String</span><span class="sxs-lookup"><span data-stu-id="453eb-145">String</span></span>|<span data-ttu-id="453eb-146">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="453eb-146">Full path, including filename.</span></span>|
|<span data-ttu-id="453eb-147">processId</span><span class="sxs-lookup"><span data-stu-id="453eb-147">processId</span></span>|<span data-ttu-id="453eb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="453eb-148">Int32</span></span>|<span data-ttu-id="453eb-149">Идентификатор процесса (PID).</span><span class="sxs-lookup"><span data-stu-id="453eb-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="453eb-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="453eb-150">JSON representation</span></span>

<span data-ttu-id="453eb-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453eb-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
