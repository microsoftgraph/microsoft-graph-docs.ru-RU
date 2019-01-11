---
title: Тип ресурса процесса
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869470"
---
# <a name="process-resource-type"></a><span data-ttu-id="1e7a7-104">Тип ресурса процесса</span><span class="sxs-lookup"><span data-stu-id="1e7a7-104">process resource type</span></span>

 > <span data-ttu-id="1e7a7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e7a7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e7a7-107">Содержит информацию о состояниях о процессе, связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1e7a7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e7a7-108">Properties</span></span>

| <span data-ttu-id="1e7a7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e7a7-109">Property</span></span>   | <span data-ttu-id="1e7a7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1e7a7-110">Type</span></span>|<span data-ttu-id="1e7a7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1e7a7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e7a7-112">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="1e7a7-112">accountName</span></span>|<span data-ttu-id="1e7a7-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1e7a7-113">String</span></span>|<span data-ttu-id="1e7a7-114">Идентификатор (учетной записи пользователя процесс запуска в разделе) учетная запись пользователя для примера, AccountName, ИД безопасности и т. д.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="1e7a7-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="1e7a7-115">commandLine</span></span>|<span data-ttu-id="1e7a7-116">String</span><span class="sxs-lookup"><span data-stu-id="1e7a7-116">String</span></span>|<span data-ttu-id="1e7a7-117">Командная строка полный процесс вызова, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="1e7a7-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e7a7-118">createdDateTime</span></span>|<span data-ttu-id="1e7a7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e7a7-119">DateTimeOffset</span></span>|<span data-ttu-id="1e7a7-120">Время начала процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-120">Time at which the process was started.</span></span> <span data-ttu-id="1e7a7-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1e7a7-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1e7a7-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1e7a7-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="1e7a7-123">fileHash</span></span>|[<span data-ttu-id="1e7a7-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="1e7a7-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="1e7a7-125">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="1e7a7-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="1e7a7-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="1e7a7-126">integrityLevel</span></span>|<span data-ttu-id="1e7a7-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="1e7a7-127">processIntegrityLevel</span></span>|<span data-ttu-id="1e7a7-128">Уровень целостности данных процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-128">The integrity level of the process.</span></span> <span data-ttu-id="1e7a7-129">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="1e7a7-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="1e7a7-130">isElevated</span></span>|<span data-ttu-id="1e7a7-131">Логический</span><span class="sxs-lookup"><span data-stu-id="1e7a7-131">Boolean</span></span>|<span data-ttu-id="1e7a7-132">Значение true, если процесс с повышенными правами.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="1e7a7-133">name</span><span class="sxs-lookup"><span data-stu-id="1e7a7-133">name</span></span>|<span data-ttu-id="1e7a7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e7a7-134">String</span></span>|<span data-ttu-id="1e7a7-135">Имя файла изображения процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="1e7a7-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e7a7-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="1e7a7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e7a7-137">DateTimeOffset</span></span>|<span data-ttu-id="1e7a7-138">Дата и время запуска родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="1e7a7-139">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1e7a7-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1e7a7-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1e7a7-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="1e7a7-141">parentProcessId</span></span>|<span data-ttu-id="1e7a7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1e7a7-142">Int32</span></span>|<span data-ttu-id="1e7a7-143">Процесс Идентификатором родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="1e7a7-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="1e7a7-144">parentProcessName</span></span>|<span data-ttu-id="1e7a7-145">Строка</span><span class="sxs-lookup"><span data-stu-id="1e7a7-145">String</span></span>|<span data-ttu-id="1e7a7-146">Имя файла изображения родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="1e7a7-147">path</span><span class="sxs-lookup"><span data-stu-id="1e7a7-147">path</span></span>|<span data-ttu-id="1e7a7-148">String</span><span class="sxs-lookup"><span data-stu-id="1e7a7-148">String</span></span>|<span data-ttu-id="1e7a7-149">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-149">Full path, including filename.</span></span>|
|<span data-ttu-id="1e7a7-150">processId</span><span class="sxs-lookup"><span data-stu-id="1e7a7-150">processId</span></span>|<span data-ttu-id="1e7a7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1e7a7-151">Int32</span></span>|<span data-ttu-id="1e7a7-152">Процесс Идентификатором процесса.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e7a7-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e7a7-153">JSON representation</span></span>

<span data-ttu-id="1e7a7-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e7a7-154">The following is a JSON representation of the resource.</span></span>

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
