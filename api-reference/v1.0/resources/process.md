---
title: тип ресурса процесса
description: Содержит сведения о процессе, связанном с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d29a09b2d593fcf1c4a3cb5bee4230e57e9836d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720732"
---
# <a name="process-resource-type"></a><span data-ttu-id="7d887-103">тип ресурса процесса</span><span class="sxs-lookup"><span data-stu-id="7d887-103">process resource type</span></span>

<span data-ttu-id="7d887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d887-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d887-105">Содержит сведения о процессе, связанном с оповещением.</span><span class="sxs-lookup"><span data-stu-id="7d887-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7d887-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d887-106">Properties</span></span>

| <span data-ttu-id="7d887-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d887-107">Property</span></span>   | <span data-ttu-id="7d887-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d887-108">Type</span></span>|<span data-ttu-id="7d887-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d887-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d887-110">accountName</span><span class="sxs-lookup"><span data-stu-id="7d887-110">accountName</span></span>|<span data-ttu-id="7d887-111">String</span><span class="sxs-lookup"><span data-stu-id="7d887-111">String</span></span>|<span data-ttu-id="7d887-112">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, в котором был указан процесс), например, Имя учетной записи, SID и так далее.</span><span class="sxs-lookup"><span data-stu-id="7d887-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="7d887-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="7d887-113">commandLine</span></span>|<span data-ttu-id="7d887-114">String</span><span class="sxs-lookup"><span data-stu-id="7d887-114">String</span></span>|<span data-ttu-id="7d887-115">Командная линия полного призыва процесса, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="7d887-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="7d887-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d887-116">createdDateTime</span></span>|<span data-ttu-id="7d887-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d887-117">DateTimeOffset</span></span>|<span data-ttu-id="7d887-118">Время начала процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-118">Time at which the process was started.</span></span> <span data-ttu-id="7d887-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7d887-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d887-120">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7d887-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="7d887-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="7d887-121">fileHash</span></span>|[<span data-ttu-id="7d887-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="7d887-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="7d887-123">Сложный тип, содержащий хеши файлов (криптографические и чувствительные к расположению).</span><span class="sxs-lookup"><span data-stu-id="7d887-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7d887-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="7d887-124">integrityLevel</span></span>|<span data-ttu-id="7d887-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="7d887-125">processIntegrityLevel</span></span>|<span data-ttu-id="7d887-126">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-126">The integrity level of the process.</span></span> <span data-ttu-id="7d887-127">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="7d887-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="7d887-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="7d887-128">isElevated</span></span>|<span data-ttu-id="7d887-129">Логический</span><span class="sxs-lookup"><span data-stu-id="7d887-129">Boolean</span></span>|<span data-ttu-id="7d887-130">True, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="7d887-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="7d887-131">name</span><span class="sxs-lookup"><span data-stu-id="7d887-131">name</span></span>|<span data-ttu-id="7d887-132">String</span><span class="sxs-lookup"><span data-stu-id="7d887-132">String</span></span>|<span data-ttu-id="7d887-133">Имя файла Image процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="7d887-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d887-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="7d887-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d887-135">DateTimeOffset</span></span>|<span data-ttu-id="7d887-136">DateTime, на котором был запущен родительский процесс.</span><span class="sxs-lookup"><span data-stu-id="7d887-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="7d887-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7d887-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d887-138">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7d887-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="7d887-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="7d887-139">parentProcessId</span></span>|<span data-ttu-id="7d887-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7d887-140">Int32</span></span>|<span data-ttu-id="7d887-141">ID процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="7d887-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="7d887-142">parentProcessName</span></span>|<span data-ttu-id="7d887-143">String</span><span class="sxs-lookup"><span data-stu-id="7d887-143">String</span></span>|<span data-ttu-id="7d887-144">Имя файла изображений родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="7d887-145">path</span><span class="sxs-lookup"><span data-stu-id="7d887-145">path</span></span>|<span data-ttu-id="7d887-146">String</span><span class="sxs-lookup"><span data-stu-id="7d887-146">String</span></span>|<span data-ttu-id="7d887-147">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="7d887-147">Full path, including filename.</span></span>|
|<span data-ttu-id="7d887-148">processId</span><span class="sxs-lookup"><span data-stu-id="7d887-148">processId</span></span>|<span data-ttu-id="7d887-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7d887-149">Int32</span></span>|<span data-ttu-id="7d887-150">ID процесса (PID) процесса.</span><span class="sxs-lookup"><span data-stu-id="7d887-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d887-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d887-151">JSON representation</span></span>

<span data-ttu-id="7d887-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d887-152">The following is a JSON representation of the resource.</span></span>

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

