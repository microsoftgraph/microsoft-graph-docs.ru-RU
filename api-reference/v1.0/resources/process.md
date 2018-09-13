# <a name="process-resource-type"></a><span data-ttu-id="7cd6a-101">Тип ресурса process</span><span class="sxs-lookup"><span data-stu-id="7cd6a-101">process resource type</span></span>

<span data-ttu-id="7cd6a-102">Содержит информацию о состоянии процесса, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-102">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7cd6a-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cd6a-103">Properties</span></span>

| <span data-ttu-id="7cd6a-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cd6a-104">Property</span></span>   | <span data-ttu-id="7cd6a-105">Тип</span><span class="sxs-lookup"><span data-stu-id="7cd6a-105">Type</span></span>|<span data-ttu-id="7cd6a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd6a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cd6a-107">accountName</span><span class="sxs-lookup"><span data-stu-id="7cd6a-107">accountName</span></span>|<span data-ttu-id="7cd6a-108">String</span><span class="sxs-lookup"><span data-stu-id="7cd6a-108">String</span></span>|<span data-ttu-id="7cd6a-109">Идентификатор учетной записи пользователя (контекст учетной записи пользователя, под которой запущен процесс), например, AccountName, ИД безопасности и т. п.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-109">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="7cd6a-110">commandLine</span><span class="sxs-lookup"><span data-stu-id="7cd6a-110">commandLine</span></span>|<span data-ttu-id="7cd6a-111">String</span><span class="sxs-lookup"><span data-stu-id="7cd6a-111">String</span></span>|<span data-ttu-id="7cd6a-112">Полная командная строка вызова процесса, включающая все параметры.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-112">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="7cd6a-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cd6a-113">createdDateTime</span></span>|<span data-ttu-id="7cd6a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cd6a-114">DateTimeOffset</span></span>|<span data-ttu-id="7cd6a-115">Время запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-115">Time at which the process was started.</span></span> <span data-ttu-id="7cd6a-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7cd6a-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7cd6a-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7cd6a-118">fileHash</span><span class="sxs-lookup"><span data-stu-id="7cd6a-118">fileHash</span></span>|[<span data-ttu-id="7cd6a-119">fileHash</span><span class="sxs-lookup"><span data-stu-id="7cd6a-119">fileHash</span></span>](filehash.md)|<span data-ttu-id="7cd6a-120">Сложный тип, содержащий хэш-значение файла (криптографическое и чувствительное к расположению).</span><span class="sxs-lookup"><span data-stu-id="7cd6a-120">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7cd6a-121">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="7cd6a-121">integrityLevel</span></span>|<span data-ttu-id="7cd6a-122">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="7cd6a-122">processIntegrityLevel</span></span>|<span data-ttu-id="7cd6a-123">Уровень целостности данных процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-123">The integrity level of the process.</span></span> <span data-ttu-id="7cd6a-124">Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-124">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="7cd6a-125">isElevated</span><span class="sxs-lookup"><span data-stu-id="7cd6a-125">isElevated</span></span>|<span data-ttu-id="7cd6a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cd6a-126">Boolean</span></span>|<span data-ttu-id="7cd6a-127">Значение true, если процесс с повышенными правами.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-127">True if the process is elevated.</span></span>|
|<span data-ttu-id="7cd6a-128">name</span><span class="sxs-lookup"><span data-stu-id="7cd6a-128">name</span></span>|<span data-ttu-id="7cd6a-129">String</span><span class="sxs-lookup"><span data-stu-id="7cd6a-129">String</span></span>|<span data-ttu-id="7cd6a-130">Имя файла образа процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-130">The name of the file.</span></span>|
|<span data-ttu-id="7cd6a-131">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cd6a-131">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="7cd6a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cd6a-132">DateTimeOffset</span></span>|<span data-ttu-id="7cd6a-133">Дата и время запуска родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-133">DateTime at which the parent process was started.</span></span> <span data-ttu-id="7cd6a-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7cd6a-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7cd6a-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7cd6a-136">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="7cd6a-136">parentProcessId</span></span>|<span data-ttu-id="7cd6a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7cd6a-137">Int32</span></span>|<span data-ttu-id="7cd6a-138">Идентификатор (PID) родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-138">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="7cd6a-139">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="7cd6a-139">parentProcessName</span></span>|<span data-ttu-id="7cd6a-140">String</span><span class="sxs-lookup"><span data-stu-id="7cd6a-140">String</span></span>|<span data-ttu-id="7cd6a-141">Имя файла образа родительского процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-141">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="7cd6a-142">path</span><span class="sxs-lookup"><span data-stu-id="7cd6a-142">path</span></span>|<span data-ttu-id="7cd6a-143">String</span><span class="sxs-lookup"><span data-stu-id="7cd6a-143">String</span></span>|<span data-ttu-id="7cd6a-144">Полный путь, включающий имя файла.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-144">Full path, including filename.</span></span>|
|<span data-ttu-id="7cd6a-145">processId</span><span class="sxs-lookup"><span data-stu-id="7cd6a-145">processId</span></span>|<span data-ttu-id="7cd6a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7cd6a-146">Int32</span></span>|<span data-ttu-id="7cd6a-147">Идентификатор (PID) процесса.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-147">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cd6a-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cd6a-148">JSON representation</span></span>

<span data-ttu-id="7cd6a-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cd6a-149">The following is a JSON representation of the resource.</span></span>

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