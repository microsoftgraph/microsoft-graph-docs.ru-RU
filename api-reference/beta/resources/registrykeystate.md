---
title: Тип ресурса registryKeyState
description: Содержит сведения об изменениях ключа реестра, связанные с оповещение и процесс, изменений в реестр.
localization_priority: Normal
ms.openlocfilehash: 688c690083e24dc6c8ee7229498910befd0fdf3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804678"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="7fc5d-103">Тип ресурса registryKeyState</span><span class="sxs-lookup"><span data-stu-id="7fc5d-103">registryKeyState resource type</span></span>

<span data-ttu-id="7fc5d-104">Содержит сведения об изменениях ключа реестра, связанные с оповещение и процесс, изменений в реестр.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="7fc5d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fc5d-105">Properties</span></span>

| <span data-ttu-id="7fc5d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fc5d-106">Property</span></span>     | <span data-ttu-id="7fc5d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7fc5d-107">Type</span></span>        | <span data-ttu-id="7fc5d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc5d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7fc5d-109">куст</span><span class="sxs-lookup"><span data-stu-id="7fc5d-109">hive</span></span>|<span data-ttu-id="7fc5d-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="7fc5d-110">registryHive</span></span>|<span data-ttu-id="7fc5d-111">[Куст реестра Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="7fc5d-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="7fc5d-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="7fc5d-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="7fc5d-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="7fc5d-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="7fc5d-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="7fc5d-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="7fc5d-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="7fc5d-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="7fc5d-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="7fc5d-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="7fc5d-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="7fc5d-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="7fc5d-118">HKEY_USERS\\. По умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="7fc5d-119">Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="7fc5d-120">key</span><span class="sxs-lookup"><span data-stu-id="7fc5d-120">key</span></span>|<span data-ttu-id="7fc5d-121">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-121">String</span></span>|<span data-ttu-id="7fc5d-122">Текущий (то есть измененные) системного реестра (исключает КУСТ).</span><span class="sxs-lookup"><span data-stu-id="7fc5d-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7fc5d-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="7fc5d-123">oldKey</span></span>|<span data-ttu-id="7fc5d-124">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-124">String</span></span>|<span data-ttu-id="7fc5d-125">Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).</span><span class="sxs-lookup"><span data-stu-id="7fc5d-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7fc5d-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="7fc5d-126">oldValueData</span></span>|<span data-ttu-id="7fc5d-127">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-127">String</span></span>|<span data-ttu-id="7fc5d-128">Предыдущий (то есть до изменения) данных значение ключа реестра (содержимое).</span><span class="sxs-lookup"><span data-stu-id="7fc5d-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7fc5d-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="7fc5d-129">oldValueName</span></span>|<span data-ttu-id="7fc5d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-130">String</span></span>|<span data-ttu-id="7fc5d-131">Предыдущий (то есть перед изменением) имя раздела реестра.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="7fc5d-132">операция</span><span class="sxs-lookup"><span data-stu-id="7fc5d-132">operation</span></span>|<span data-ttu-id="7fc5d-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="7fc5d-133">registryOperation</span></span>|<span data-ttu-id="7fc5d-134">Операция, изменено имя раздела реестра и/или значение.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="7fc5d-135">Возможные значения: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="7fc5d-136">processId</span><span class="sxs-lookup"><span data-stu-id="7fc5d-136">processId</span></span>|<span data-ttu-id="7fc5d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7fc5d-137">Int32</span></span>|<span data-ttu-id="7fc5d-138">Обработать Идентификатором процесса изменения раздела реестра (процесс отображения сведений в коллекции оповещения «процессы»).</span><span class="sxs-lookup"><span data-stu-id="7fc5d-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="7fc5d-139">valueData</span><span class="sxs-lookup"><span data-stu-id="7fc5d-139">valueData</span></span>|<span data-ttu-id="7fc5d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-140">String</span></span>|<span data-ttu-id="7fc5d-141">Текущий (то есть измененные) значение ключа реестра (содержимое).</span><span class="sxs-lookup"><span data-stu-id="7fc5d-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7fc5d-142">Имени</span><span class="sxs-lookup"><span data-stu-id="7fc5d-142">valueName</span></span>|<span data-ttu-id="7fc5d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc5d-143">String</span></span>|<span data-ttu-id="7fc5d-144">Текущее имя значение ключа реестра (то есть измененные)</span><span class="sxs-lookup"><span data-stu-id="7fc5d-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="7fc5d-145">Тип значения</span><span class="sxs-lookup"><span data-stu-id="7fc5d-145">valueType</span></span>|<span data-ttu-id="7fc5d-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="7fc5d-146">registryValueType</span></span>|[<span data-ttu-id="7fc5d-147">Тип значения ключа реестра</span><span class="sxs-lookup"><span data-stu-id="7fc5d-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="7fc5d-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="7fc5d-148">REG_BINARY</span></span></li> <li><span data-ttu-id="7fc5d-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7fc5d-149">REG_DWORD</span></span></li> <li><span data-ttu-id="7fc5d-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7fc5d-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7fc5d-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7fc5d-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="7fc5d-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="7fc5d-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="7fc5d-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="7fc5d-153">REG_LINK</span></span></li> <li><span data-ttu-id="7fc5d-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="7fc5d-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="7fc5d-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="7fc5d-155">REG_NONE</span></span></li> <li><span data-ttu-id="7fc5d-156">REG_QWORD ИНТЕРФЕЙСА</span><span class="sxs-lookup"><span data-stu-id="7fc5d-156">REG_QWORD</span></span></li> <li><span data-ttu-id="7fc5d-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7fc5d-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7fc5d-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="7fc5d-158">REG_SZ</span></span></li></ul> <span data-ttu-id="7fc5d-159">Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fc5d-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7fc5d-160">JSON representation</span></span>

<span data-ttu-id="7fc5d-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fc5d-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
