---
title: Тип ресурса "процесс"
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 244c809008eaea286f3048ed103d1b5320e0765e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344294"
---
# <a name="process-resource-type"></a><span data-ttu-id="4a72a-104">Тип ресурса "процесс"</span><span class="sxs-lookup"><span data-stu-id="4a72a-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a72a-105">Содержит сведения о состоянии процесса, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="4a72a-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="4a72a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a72a-106">Properties</span></span>

| <span data-ttu-id="4a72a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a72a-107">Property</span></span>   | <span data-ttu-id="4a72a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4a72a-108">Type</span></span>|<span data-ttu-id="4a72a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a72a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a72a-110">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="4a72a-110">accountName</span></span>|<span data-ttu-id="4a72a-111">String</span><span class="sxs-lookup"><span data-stu-id="4a72a-111">String</span></span>|<span data-ttu-id="4a72a-112">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, который выполнялся в данный процесс) например, имя_учетной_записи, SID и т. д.</span><span class="sxs-lookup"><span data-stu-id="4a72a-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="4a72a-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="4a72a-113">commandLine</span></span>|<span data-ttu-id="4a72a-114">String</span><span class="sxs-lookup"><span data-stu-id="4a72a-114">String</span></span>|<span data-ttu-id="4a72a-115">Командная строка вызова полной обработки, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="4a72a-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="4a72a-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a72a-116">createdDateTime</span></span>|<span data-ttu-id="4a72a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a72a-117">DateTimeOffset</span></span>|<span data-ttu-id="4a72a-118">Время запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-118">Time at which the process was started.</span></span> <span data-ttu-id="4a72a-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4a72a-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a72a-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4a72a-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4a72a-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="4a72a-121">fileHash</span></span>|[<span data-ttu-id="4a72a-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="4a72a-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="4a72a-123">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="4a72a-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="4a72a-124">Интегритилевел</span><span class="sxs-lookup"><span data-stu-id="4a72a-124">integrityLevel</span></span>|<span data-ttu-id="4a72a-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="4a72a-125">processIntegrityLevel</span></span>|<span data-ttu-id="4a72a-126">Уровень целостности процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-126">The integrity level of the process.</span></span> <span data-ttu-id="4a72a-127">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="4a72a-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="4a72a-128">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="4a72a-128">isElevated</span></span>|<span data-ttu-id="4a72a-129">Логический</span><span class="sxs-lookup"><span data-stu-id="4a72a-129">Boolean</span></span>|<span data-ttu-id="4a72a-130">Значение true, если процесс повышен.</span><span class="sxs-lookup"><span data-stu-id="4a72a-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="4a72a-131">name</span><span class="sxs-lookup"><span data-stu-id="4a72a-131">name</span></span>|<span data-ttu-id="4a72a-132">String</span><span class="sxs-lookup"><span data-stu-id="4a72a-132">String</span></span>|<span data-ttu-id="4a72a-133">Имя файла образа процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="4a72a-134">Парентпроцесскреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="4a72a-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="4a72a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a72a-135">DateTimeOffset</span></span>|<span data-ttu-id="4a72a-136">Дата и время начала родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="4a72a-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4a72a-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a72a-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4a72a-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4a72a-139">Парентпроцессид</span><span class="sxs-lookup"><span data-stu-id="4a72a-139">parentProcessId</span></span>|<span data-ttu-id="4a72a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4a72a-140">Int32</span></span>|<span data-ttu-id="4a72a-141">Идентификатор процесса (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="4a72a-142">Парентпроцесснаме</span><span class="sxs-lookup"><span data-stu-id="4a72a-142">parentProcessName</span></span>|<span data-ttu-id="4a72a-143">String</span><span class="sxs-lookup"><span data-stu-id="4a72a-143">String</span></span>|<span data-ttu-id="4a72a-144">Имя файла образа родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="4a72a-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="4a72a-145">path</span><span class="sxs-lookup"><span data-stu-id="4a72a-145">path</span></span>|<span data-ttu-id="4a72a-146">String</span><span class="sxs-lookup"><span data-stu-id="4a72a-146">String</span></span>|<span data-ttu-id="4a72a-147">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="4a72a-147">Full path, including filename.</span></span>|
|<span data-ttu-id="4a72a-148">processId</span><span class="sxs-lookup"><span data-stu-id="4a72a-148">processId</span></span>|<span data-ttu-id="4a72a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4a72a-149">Int32</span></span>|<span data-ttu-id="4a72a-150">Идентификатор процесса (PID).</span><span class="sxs-lookup"><span data-stu-id="4a72a-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a72a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a72a-151">JSON representation</span></span>

<span data-ttu-id="4a72a-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a72a-152">The following is a JSON representation of the resource.</span></span>

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
