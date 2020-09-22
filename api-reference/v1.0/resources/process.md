---
title: Тип ресурса "процесс"
description: Содержит сведения о состоянии процесса, связанного с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f895ccbc1aaa143bbc9bb8adc7045fbab705e0cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037229"
---
# <a name="process-resource-type"></a><span data-ttu-id="de5be-103">Тип ресурса "процесс"</span><span class="sxs-lookup"><span data-stu-id="de5be-103">process resource type</span></span>

<span data-ttu-id="de5be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de5be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de5be-105">Содержит сведения о состоянии процесса, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="de5be-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="de5be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="de5be-106">Properties</span></span>

| <span data-ttu-id="de5be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="de5be-107">Property</span></span>   | <span data-ttu-id="de5be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="de5be-108">Type</span></span>|<span data-ttu-id="de5be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de5be-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de5be-110">accountName</span><span class="sxs-lookup"><span data-stu-id="de5be-110">accountName</span></span>|<span data-ttu-id="de5be-111">String</span><span class="sxs-lookup"><span data-stu-id="de5be-111">String</span></span>|<span data-ttu-id="de5be-112">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, который выполнялся в данный процесс) например, имя_учетной_записи, SID и т. д.</span><span class="sxs-lookup"><span data-stu-id="de5be-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="de5be-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="de5be-113">commandLine</span></span>|<span data-ttu-id="de5be-114">String</span><span class="sxs-lookup"><span data-stu-id="de5be-114">String</span></span>|<span data-ttu-id="de5be-115">Командная строка вызова полной обработки, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="de5be-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="de5be-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de5be-116">createdDateTime</span></span>|<span data-ttu-id="de5be-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de5be-117">DateTimeOffset</span></span>|<span data-ttu-id="de5be-118">Время запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-118">Time at which the process was started.</span></span> <span data-ttu-id="de5be-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="de5be-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de5be-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="de5be-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="de5be-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="de5be-121">fileHash</span></span>|[<span data-ttu-id="de5be-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="de5be-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="de5be-123">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="de5be-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="de5be-124">интегритилевел</span><span class="sxs-lookup"><span data-stu-id="de5be-124">integrityLevel</span></span>|<span data-ttu-id="de5be-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="de5be-125">processIntegrityLevel</span></span>|<span data-ttu-id="de5be-126">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-126">The integrity level of the process.</span></span> <span data-ttu-id="de5be-127">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="de5be-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="de5be-128">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="de5be-128">isElevated</span></span>|<span data-ttu-id="de5be-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="de5be-129">Boolean</span></span>|<span data-ttu-id="de5be-130">Значение true, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="de5be-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="de5be-131">name</span><span class="sxs-lookup"><span data-stu-id="de5be-131">name</span></span>|<span data-ttu-id="de5be-132">String</span><span class="sxs-lookup"><span data-stu-id="de5be-132">String</span></span>|<span data-ttu-id="de5be-133">Имя файла образа процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="de5be-134">парентпроцесскреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="de5be-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="de5be-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de5be-135">DateTimeOffset</span></span>|<span data-ttu-id="de5be-136">Дата и время начала родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="de5be-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="de5be-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de5be-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="de5be-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="de5be-139">парентпроцессид</span><span class="sxs-lookup"><span data-stu-id="de5be-139">parentProcessId</span></span>|<span data-ttu-id="de5be-140">Int32</span><span class="sxs-lookup"><span data-stu-id="de5be-140">Int32</span></span>|<span data-ttu-id="de5be-141">Идентификатор процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="de5be-142">парентпроцесснаме</span><span class="sxs-lookup"><span data-stu-id="de5be-142">parentProcessName</span></span>|<span data-ttu-id="de5be-143">String</span><span class="sxs-lookup"><span data-stu-id="de5be-143">String</span></span>|<span data-ttu-id="de5be-144">Имя файла образа родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="de5be-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="de5be-145">path</span><span class="sxs-lookup"><span data-stu-id="de5be-145">path</span></span>|<span data-ttu-id="de5be-146">String</span><span class="sxs-lookup"><span data-stu-id="de5be-146">String</span></span>|<span data-ttu-id="de5be-147">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="de5be-147">Full path, including filename.</span></span>|
|<span data-ttu-id="de5be-148">processId</span><span class="sxs-lookup"><span data-stu-id="de5be-148">processId</span></span>|<span data-ttu-id="de5be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="de5be-149">Int32</span></span>|<span data-ttu-id="de5be-150">Идентификатор процесса (PID).</span><span class="sxs-lookup"><span data-stu-id="de5be-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de5be-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de5be-151">JSON representation</span></span>

<span data-ttu-id="de5be-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de5be-152">The following is a JSON representation of the resource.</span></span>

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

