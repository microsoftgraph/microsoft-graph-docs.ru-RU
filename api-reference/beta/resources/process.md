---
title: тип ресурса процесса
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: db832c64fb62e6c5f72f49b1e147d8d7f282834f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722274"
---
# <a name="process-resource-type"></a><span data-ttu-id="902e2-104">тип ресурса процесса</span><span class="sxs-lookup"><span data-stu-id="902e2-104">process resource type</span></span>

<span data-ttu-id="902e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="902e2-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="902e2-106">Содержит сведения о процессе, связанном с оповещением.</span><span class="sxs-lookup"><span data-stu-id="902e2-106">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="902e2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="902e2-107">Properties</span></span>

| <span data-ttu-id="902e2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="902e2-108">Property</span></span>   | <span data-ttu-id="902e2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="902e2-109">Type</span></span>|<span data-ttu-id="902e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="902e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="902e2-111">accountName</span><span class="sxs-lookup"><span data-stu-id="902e2-111">accountName</span></span>|<span data-ttu-id="902e2-112">String</span><span class="sxs-lookup"><span data-stu-id="902e2-112">String</span></span>|<span data-ttu-id="902e2-113">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, в котором был указан процесс), например, Имя учетной записи, SID и так далее.</span><span class="sxs-lookup"><span data-stu-id="902e2-113">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="902e2-114">commandLine</span><span class="sxs-lookup"><span data-stu-id="902e2-114">commandLine</span></span>|<span data-ttu-id="902e2-115">String</span><span class="sxs-lookup"><span data-stu-id="902e2-115">String</span></span>|<span data-ttu-id="902e2-116">Командная линия полного призыва процесса, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="902e2-116">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="902e2-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="902e2-117">createdDateTime</span></span>|<span data-ttu-id="902e2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="902e2-118">DateTimeOffset</span></span>|<span data-ttu-id="902e2-119">Время начала процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-119">Time at which the process was started.</span></span> <span data-ttu-id="902e2-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="902e2-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="902e2-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="902e2-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="902e2-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="902e2-122">fileHash</span></span>|[<span data-ttu-id="902e2-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="902e2-123">fileHash</span></span>](filehash.md)|<span data-ttu-id="902e2-124">Сложный тип, содержащий хеши файлов (криптографические и чувствительные к расположению).</span><span class="sxs-lookup"><span data-stu-id="902e2-124">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="902e2-125">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="902e2-125">integrityLevel</span></span>|<span data-ttu-id="902e2-126">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="902e2-126">processIntegrityLevel</span></span>|<span data-ttu-id="902e2-127">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-127">The integrity level of the process.</span></span> <span data-ttu-id="902e2-128">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="902e2-128">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="902e2-129">isElevated</span><span class="sxs-lookup"><span data-stu-id="902e2-129">isElevated</span></span>|<span data-ttu-id="902e2-130">Логический</span><span class="sxs-lookup"><span data-stu-id="902e2-130">Boolean</span></span>|<span data-ttu-id="902e2-131">True, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="902e2-131">True if the process is elevated.</span></span>|
|<span data-ttu-id="902e2-132">name</span><span class="sxs-lookup"><span data-stu-id="902e2-132">name</span></span>|<span data-ttu-id="902e2-133">String</span><span class="sxs-lookup"><span data-stu-id="902e2-133">String</span></span>|<span data-ttu-id="902e2-134">Имя файла Image процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-134">The name of the process' Image file.</span></span>|
|<span data-ttu-id="902e2-135">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="902e2-135">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="902e2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="902e2-136">DateTimeOffset</span></span>|<span data-ttu-id="902e2-137">DateTime, на котором был запущен родительский процесс.</span><span class="sxs-lookup"><span data-stu-id="902e2-137">DateTime at which the parent process was started.</span></span> <span data-ttu-id="902e2-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="902e2-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="902e2-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="902e2-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="902e2-140">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="902e2-140">parentProcessId</span></span>|<span data-ttu-id="902e2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="902e2-141">Int32</span></span>|<span data-ttu-id="902e2-142">ID процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-142">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="902e2-143">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="902e2-143">parentProcessName</span></span>|<span data-ttu-id="902e2-144">String</span><span class="sxs-lookup"><span data-stu-id="902e2-144">String</span></span>|<span data-ttu-id="902e2-145">Имя файла изображений родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-145">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="902e2-146">path</span><span class="sxs-lookup"><span data-stu-id="902e2-146">path</span></span>|<span data-ttu-id="902e2-147">String</span><span class="sxs-lookup"><span data-stu-id="902e2-147">String</span></span>|<span data-ttu-id="902e2-148">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="902e2-148">Full path, including filename.</span></span>|
|<span data-ttu-id="902e2-149">processId</span><span class="sxs-lookup"><span data-stu-id="902e2-149">processId</span></span>|<span data-ttu-id="902e2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="902e2-150">Int32</span></span>|<span data-ttu-id="902e2-151">ID процесса (PID) процесса.</span><span class="sxs-lookup"><span data-stu-id="902e2-151">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="902e2-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="902e2-152">JSON representation</span></span>

<span data-ttu-id="902e2-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902e2-153">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


