---
title: Тип ресурса "процесс"
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6fb3ec0651ab920b27d29fd95475e0125accdf10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521483"
---
# <a name="process-resource-type"></a><span data-ttu-id="9fd0b-104">Тип ресурса "процесс"</span><span class="sxs-lookup"><span data-stu-id="9fd0b-104">process resource type</span></span>

<span data-ttu-id="9fd0b-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9fd0b-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd0b-106">Содержит сведения о состоянии процесса, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-106">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9fd0b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fd0b-107">Properties</span></span>

| <span data-ttu-id="9fd0b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fd0b-108">Property</span></span>   | <span data-ttu-id="9fd0b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9fd0b-109">Type</span></span>|<span data-ttu-id="9fd0b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd0b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fd0b-111">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="9fd0b-111">accountName</span></span>|<span data-ttu-id="9fd0b-112">String</span><span class="sxs-lookup"><span data-stu-id="9fd0b-112">String</span></span>|<span data-ttu-id="9fd0b-113">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, который выполнялся в данный процесс) например, имя_учетной_записи, SID и т. д.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-113">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="9fd0b-114">commandLine</span><span class="sxs-lookup"><span data-stu-id="9fd0b-114">commandLine</span></span>|<span data-ttu-id="9fd0b-115">String</span><span class="sxs-lookup"><span data-stu-id="9fd0b-115">String</span></span>|<span data-ttu-id="9fd0b-116">Командная строка вызова полной обработки, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-116">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="9fd0b-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fd0b-117">createdDateTime</span></span>|<span data-ttu-id="9fd0b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd0b-118">DateTimeOffset</span></span>|<span data-ttu-id="9fd0b-119">Время запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-119">Time at which the process was started.</span></span> <span data-ttu-id="9fd0b-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9fd0b-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fd0b-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9fd0b-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="9fd0b-122">fileHash</span></span>|[<span data-ttu-id="9fd0b-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="9fd0b-123">fileHash</span></span>](filehash.md)|<span data-ttu-id="9fd0b-124">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="9fd0b-124">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="9fd0b-125">интегритилевел</span><span class="sxs-lookup"><span data-stu-id="9fd0b-125">integrityLevel</span></span>|<span data-ttu-id="9fd0b-126">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="9fd0b-126">processIntegrityLevel</span></span>|<span data-ttu-id="9fd0b-127">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-127">The integrity level of the process.</span></span> <span data-ttu-id="9fd0b-128">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-128">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="9fd0b-129">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="9fd0b-129">isElevated</span></span>|<span data-ttu-id="9fd0b-130">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd0b-130">Boolean</span></span>|<span data-ttu-id="9fd0b-131">Значение true, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-131">True if the process is elevated.</span></span>|
|<span data-ttu-id="9fd0b-132">name</span><span class="sxs-lookup"><span data-stu-id="9fd0b-132">name</span></span>|<span data-ttu-id="9fd0b-133">String</span><span class="sxs-lookup"><span data-stu-id="9fd0b-133">String</span></span>|<span data-ttu-id="9fd0b-134">Имя файла образа процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-134">The name of the process' Image file.</span></span>|
|<span data-ttu-id="9fd0b-135">парентпроцесскреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="9fd0b-135">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="9fd0b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd0b-136">DateTimeOffset</span></span>|<span data-ttu-id="9fd0b-137">Дата и время начала родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-137">DateTime at which the parent process was started.</span></span> <span data-ttu-id="9fd0b-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9fd0b-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fd0b-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9fd0b-140">парентпроцессид</span><span class="sxs-lookup"><span data-stu-id="9fd0b-140">parentProcessId</span></span>|<span data-ttu-id="9fd0b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9fd0b-141">Int32</span></span>|<span data-ttu-id="9fd0b-142">Идентификатор процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-142">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="9fd0b-143">парентпроцесснаме</span><span class="sxs-lookup"><span data-stu-id="9fd0b-143">parentProcessName</span></span>|<span data-ttu-id="9fd0b-144">String</span><span class="sxs-lookup"><span data-stu-id="9fd0b-144">String</span></span>|<span data-ttu-id="9fd0b-145">Имя файла образа родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-145">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="9fd0b-146">path</span><span class="sxs-lookup"><span data-stu-id="9fd0b-146">path</span></span>|<span data-ttu-id="9fd0b-147">String</span><span class="sxs-lookup"><span data-stu-id="9fd0b-147">String</span></span>|<span data-ttu-id="9fd0b-148">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-148">Full path, including filename.</span></span>|
|<span data-ttu-id="9fd0b-149">processId</span><span class="sxs-lookup"><span data-stu-id="9fd0b-149">processId</span></span>|<span data-ttu-id="9fd0b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9fd0b-150">Int32</span></span>|<span data-ttu-id="9fd0b-151">Идентификатор процесса (PID).</span><span class="sxs-lookup"><span data-stu-id="9fd0b-151">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fd0b-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fd0b-152">JSON representation</span></span>

<span data-ttu-id="9fd0b-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd0b-153">The following is a JSON representation of the resource.</span></span>

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
