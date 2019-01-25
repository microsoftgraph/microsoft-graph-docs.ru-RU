---
title: Тип ресурса процесса
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521210"
---
# <a name="process-resource-type"></a><span data-ttu-id="aba60-104">Тип ресурса процесса</span><span class="sxs-lookup"><span data-stu-id="aba60-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba60-105">Содержит информацию о состояниях о процессе, связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="aba60-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="aba60-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aba60-106">Properties</span></span>

| <span data-ttu-id="aba60-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aba60-107">Property</span></span>   | <span data-ttu-id="aba60-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aba60-108">Type</span></span>|<span data-ttu-id="aba60-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aba60-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aba60-110">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="aba60-110">accountName</span></span>|<span data-ttu-id="aba60-111">String</span><span class="sxs-lookup"><span data-stu-id="aba60-111">String</span></span>|<span data-ttu-id="aba60-112">Идентификатор (учетной записи пользователя процесс запуска в разделе) учетная запись пользователя для примера, AccountName, ИД безопасности и т. д.</span><span class="sxs-lookup"><span data-stu-id="aba60-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="aba60-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="aba60-113">commandLine</span></span>|<span data-ttu-id="aba60-114">String</span><span class="sxs-lookup"><span data-stu-id="aba60-114">String</span></span>|<span data-ttu-id="aba60-115">Командная строка полный процесс вызова, включая все параметры.</span><span class="sxs-lookup"><span data-stu-id="aba60-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="aba60-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aba60-116">createdDateTime</span></span>|<span data-ttu-id="aba60-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aba60-117">DateTimeOffset</span></span>|<span data-ttu-id="aba60-118">Время начала процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-118">Time at which the process was started.</span></span> <span data-ttu-id="aba60-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aba60-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aba60-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aba60-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aba60-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="aba60-121">fileHash</span></span>|[<span data-ttu-id="aba60-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="aba60-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="aba60-123">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="aba60-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="aba60-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="aba60-124">integrityLevel</span></span>|<span data-ttu-id="aba60-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="aba60-125">processIntegrityLevel</span></span>|<span data-ttu-id="aba60-126">Уровень целостности данных процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-126">The integrity level of the process.</span></span> <span data-ttu-id="aba60-127">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="aba60-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="aba60-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="aba60-128">isElevated</span></span>|<span data-ttu-id="aba60-129">Логическое</span><span class="sxs-lookup"><span data-stu-id="aba60-129">Boolean</span></span>|<span data-ttu-id="aba60-130">Значение true, если процесс с повышенными правами.</span><span class="sxs-lookup"><span data-stu-id="aba60-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="aba60-131">name</span><span class="sxs-lookup"><span data-stu-id="aba60-131">name</span></span>|<span data-ttu-id="aba60-132">String</span><span class="sxs-lookup"><span data-stu-id="aba60-132">String</span></span>|<span data-ttu-id="aba60-133">Имя файла изображения процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="aba60-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="aba60-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="aba60-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aba60-135">DateTimeOffset</span></span>|<span data-ttu-id="aba60-136">Дата и время запуска родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="aba60-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aba60-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aba60-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aba60-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aba60-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="aba60-139">parentProcessId</span></span>|<span data-ttu-id="aba60-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aba60-140">Int32</span></span>|<span data-ttu-id="aba60-141">Процесс Идентификатором родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="aba60-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="aba60-142">parentProcessName</span></span>|<span data-ttu-id="aba60-143">String</span><span class="sxs-lookup"><span data-stu-id="aba60-143">String</span></span>|<span data-ttu-id="aba60-144">Имя файла изображения родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="aba60-145">path</span><span class="sxs-lookup"><span data-stu-id="aba60-145">path</span></span>|<span data-ttu-id="aba60-146">String</span><span class="sxs-lookup"><span data-stu-id="aba60-146">String</span></span>|<span data-ttu-id="aba60-147">Полный путь, включая имя файла.</span><span class="sxs-lookup"><span data-stu-id="aba60-147">Full path, including filename.</span></span>|
|<span data-ttu-id="aba60-148">ProcessID</span><span class="sxs-lookup"><span data-stu-id="aba60-148">processId</span></span>|<span data-ttu-id="aba60-149">Int32</span><span class="sxs-lookup"><span data-stu-id="aba60-149">Int32</span></span>|<span data-ttu-id="aba60-150">Процесс Идентификатором процесса.</span><span class="sxs-lookup"><span data-stu-id="aba60-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aba60-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aba60-151">JSON representation</span></span>

<span data-ttu-id="aba60-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aba60-152">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
