---
title: Тип ресурса Регистрикэйстате
description: Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b07f031fed393c4de41a55b55e8009ca9c8d8259
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806795"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="b00d5-103">Тип ресурса Регистрикэйстате</span><span class="sxs-lookup"><span data-stu-id="b00d5-103">registryKeyState resource type</span></span>

<span data-ttu-id="b00d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b00d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b00d5-105">Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="b00d5-105">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="b00d5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b00d5-106">Properties</span></span>

| <span data-ttu-id="b00d5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b00d5-107">Property</span></span>     | <span data-ttu-id="b00d5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b00d5-108">Type</span></span>        | <span data-ttu-id="b00d5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b00d5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b00d5-110">семейства</span><span class="sxs-lookup"><span data-stu-id="b00d5-110">hive</span></span>|<span data-ttu-id="b00d5-111">registryHive</span><span class="sxs-lookup"><span data-stu-id="b00d5-111">registryHive</span></span>|<span data-ttu-id="b00d5-112">[Куст реестра Windows](/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="b00d5-112">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="b00d5-113">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="b00d5-113">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="b00d5-114">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="b00d5-114">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="b00d5-115">HKEY_LOCAL_MACHINE \САМ</span><span class="sxs-lookup"><span data-stu-id="b00d5-115">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="b00d5-116">HKEY_LOCAL_MACHINE \Секурити</span><span class="sxs-lookup"><span data-stu-id="b00d5-116">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="b00d5-117">HKEY_LOCAL_MACHINE \Софтваре</span><span class="sxs-lookup"><span data-stu-id="b00d5-117">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="b00d5-118">HKEY_LOCAL_MACHINE \Систем</span><span class="sxs-lookup"><span data-stu-id="b00d5-118">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="b00d5-119">HKEY_USERS \\ . Умолчани.</span><span class="sxs-lookup"><span data-stu-id="b00d5-119">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="b00d5-120">Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="b00d5-120">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="b00d5-121">ключа</span><span class="sxs-lookup"><span data-stu-id="b00d5-121">key</span></span>|<span data-ttu-id="b00d5-122">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-122">String</span></span>|<span data-ttu-id="b00d5-123">Текущий (то есть измененный) раздел реестра (исключая КУСТ).</span><span class="sxs-lookup"><span data-stu-id="b00d5-123">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="b00d5-124">олдкэй</span><span class="sxs-lookup"><span data-stu-id="b00d5-124">oldKey</span></span>|<span data-ttu-id="b00d5-125">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-125">String</span></span>|<span data-ttu-id="b00d5-126">Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).</span><span class="sxs-lookup"><span data-stu-id="b00d5-126">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="b00d5-127">олдвалуедата</span><span class="sxs-lookup"><span data-stu-id="b00d5-127">oldValueData</span></span>|<span data-ttu-id="b00d5-128">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-128">String</span></span>|<span data-ttu-id="b00d5-129">Previous (то есть перед изменением) значение раздела реестра (Content).</span><span class="sxs-lookup"><span data-stu-id="b00d5-129">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="b00d5-130">олдвалуенаме</span><span class="sxs-lookup"><span data-stu-id="b00d5-130">oldValueName</span></span>|<span data-ttu-id="b00d5-131">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-131">String</span></span>|<span data-ttu-id="b00d5-132">Previous (то есть перед изменением) имя значения раздела реестра.</span><span class="sxs-lookup"><span data-stu-id="b00d5-132">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="b00d5-133">восстановление</span><span class="sxs-lookup"><span data-stu-id="b00d5-133">operation</span></span>|<span data-ttu-id="b00d5-134">registryOperation</span><span class="sxs-lookup"><span data-stu-id="b00d5-134">registryOperation</span></span>|<span data-ttu-id="b00d5-135">Операция, в которой изменилось имя и/или значение раздела реестра.</span><span class="sxs-lookup"><span data-stu-id="b00d5-135">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="b00d5-136">Возможные значения: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="b00d5-136">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="b00d5-137">processId</span><span class="sxs-lookup"><span data-stu-id="b00d5-137">processId</span></span>|<span data-ttu-id="b00d5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b00d5-138">Int32</span></span>|<span data-ttu-id="b00d5-139">Идентификатор процесса (PID), который изменил раздел реестра (сведения о процессе будут отображаться в коллекции предупреждений "процессы").</span><span class="sxs-lookup"><span data-stu-id="b00d5-139">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="b00d5-140">валуедата</span><span class="sxs-lookup"><span data-stu-id="b00d5-140">valueData</span></span>|<span data-ttu-id="b00d5-141">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-141">String</span></span>|<span data-ttu-id="b00d5-142">Текущие (то есть измененные) данные значения раздела реестра (содержимое).</span><span class="sxs-lookup"><span data-stu-id="b00d5-142">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="b00d5-143">valueName</span><span class="sxs-lookup"><span data-stu-id="b00d5-143">valueName</span></span>|<span data-ttu-id="b00d5-144">String</span><span class="sxs-lookup"><span data-stu-id="b00d5-144">String</span></span>|<span data-ttu-id="b00d5-145">Current (то есть изменено) имя значения раздела реестра</span><span class="sxs-lookup"><span data-stu-id="b00d5-145">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="b00d5-146">Типом</span><span class="sxs-lookup"><span data-stu-id="b00d5-146">valueType</span></span>|<span data-ttu-id="b00d5-147">registryValueType</span><span class="sxs-lookup"><span data-stu-id="b00d5-147">registryValueType</span></span>|[<span data-ttu-id="b00d5-148">Тип значения раздела реестра</span><span class="sxs-lookup"><span data-stu-id="b00d5-148">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="b00d5-149">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="b00d5-149">REG_BINARY</span></span></li> <li><span data-ttu-id="b00d5-150">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b00d5-150">REG_DWORD</span></span></li> <li><span data-ttu-id="b00d5-151">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b00d5-151">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="b00d5-152">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b00d5-152">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="b00d5-153">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="b00d5-153">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="b00d5-154">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="b00d5-154">REG_LINK</span></span></li> <li><span data-ttu-id="b00d5-155">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="b00d5-155">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="b00d5-156">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="b00d5-156">REG_NONE</span></span></li> <li><span data-ttu-id="b00d5-157">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="b00d5-157">REG_QWORD</span></span></li> <li><span data-ttu-id="b00d5-158">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b00d5-158">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="b00d5-159">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="b00d5-159">REG_SZ</span></span></li></ul> <span data-ttu-id="b00d5-160">Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="b00d5-160">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b00d5-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b00d5-161">JSON representation</span></span>

<span data-ttu-id="b00d5-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b00d5-162">The following is a JSON representation of the resource.</span></span>

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
