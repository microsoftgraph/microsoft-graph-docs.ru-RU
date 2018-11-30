---
title: Тип ресурса процесса
description: Содержит информацию о состояниях о процессе, связанные с оповещение.
ms.openlocfilehash: 67bc65cfa47cda877578d89aa20c4e34b3a0c501
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027330"
---
# <a name="process-resource-type"></a><span data-ttu-id="12e1c-103">Тип ресурса процесса</span><span class="sxs-lookup"><span data-stu-id="12e1c-103">process resource type</span></span>

<span data-ttu-id="12e1c-104">Содержит информацию о состояниях о процессе, связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="12e1c-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="12e1c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="12e1c-105">Properties</span></span>

| <span data-ttu-id="12e1c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="12e1c-106">Property</span></span>   | <span data-ttu-id="12e1c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="12e1c-107">Type</span></span>|<span data-ttu-id="12e1c-108">Description</span><span class="sxs-lookup"><span data-stu-id="12e1c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e1c-109">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="12e1c-109">accountName</span></span>|<span data-ttu-id="12e1c-110">String</span><span class="sxs-lookup"><span data-stu-id="12e1c-110">String</span></span>|<span data-ttu-id="12e1c-111">Идентификатор (учетной записи пользователя процесс запуска в разделе) учетная запись пользователя для примера, AccountName, ИД безопасности и т. д.</span><span class="sxs-lookup"><span data-stu-id="12e1c-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="12e1c-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="12e1c-112">commandLine</span></span>|<span data-ttu-id="12e1c-113">String</span><span class="sxs-lookup"><span data-stu-id="12e1c-113">String</span></span>|<span data-ttu-id="12e1c-114">Командная строка полный процесс вызова, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="12e1c-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="12e1c-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12e1c-115">createdDateTime</span></span>|<span data-ttu-id="12e1c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12e1c-116">DateTimeOffset</span></span>|<span data-ttu-id="12e1c-117">Время начала процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-117">Time at which the process was started.</span></span> <span data-ttu-id="12e1c-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="12e1c-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12e1c-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12e1c-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="12e1c-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="12e1c-120">fileHash</span></span>|[<span data-ttu-id="12e1c-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="12e1c-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="12e1c-122">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="12e1c-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="12e1c-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="12e1c-123">integrityLevel</span></span>|<span data-ttu-id="12e1c-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="12e1c-124">processIntegrityLevel</span></span>|<span data-ttu-id="12e1c-125">Уровень целостности данных процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-125">The integrity level of the process.</span></span> <span data-ttu-id="12e1c-126">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="12e1c-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="12e1c-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="12e1c-127">isElevated</span></span>|<span data-ttu-id="12e1c-128">Логический</span><span class="sxs-lookup"><span data-stu-id="12e1c-128">Boolean</span></span>|<span data-ttu-id="12e1c-129">Значение true, если процесс с повышенными правами.</span><span class="sxs-lookup"><span data-stu-id="12e1c-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="12e1c-130">name</span><span class="sxs-lookup"><span data-stu-id="12e1c-130">name</span></span>|<span data-ttu-id="12e1c-131">String</span><span class="sxs-lookup"><span data-stu-id="12e1c-131">String</span></span>|<span data-ttu-id="12e1c-132">Имя файла изображения процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="12e1c-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="12e1c-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="12e1c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12e1c-134">DateTimeOffset</span></span>|<span data-ttu-id="12e1c-135">Дата и время запуска родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="12e1c-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="12e1c-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12e1c-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12e1c-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="12e1c-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="12e1c-138">parentProcessId</span></span>|<span data-ttu-id="12e1c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="12e1c-139">Int32</span></span>|<span data-ttu-id="12e1c-140">Процесс Идентификатором родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="12e1c-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="12e1c-141">parentProcessName</span></span>|<span data-ttu-id="12e1c-142">String</span><span class="sxs-lookup"><span data-stu-id="12e1c-142">String</span></span>|<span data-ttu-id="12e1c-143">Имя файла изображения родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="12e1c-144">path</span><span class="sxs-lookup"><span data-stu-id="12e1c-144">path</span></span>|<span data-ttu-id="12e1c-145">String</span><span class="sxs-lookup"><span data-stu-id="12e1c-145">String</span></span>|<span data-ttu-id="12e1c-146">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="12e1c-146">Full path, including filename.</span></span>|
|<span data-ttu-id="12e1c-147">processId</span><span class="sxs-lookup"><span data-stu-id="12e1c-147">processId</span></span>|<span data-ttu-id="12e1c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="12e1c-148">Int32</span></span>|<span data-ttu-id="12e1c-149">Процесс Идентификатором процесса.</span><span class="sxs-lookup"><span data-stu-id="12e1c-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12e1c-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12e1c-150">JSON representation</span></span>

<span data-ttu-id="12e1c-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12e1c-151">The following is a JSON representation of the resource.</span></span>

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