---
title: Тип ресурса Регистрикэйстате
description: Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e685bc281344f05a43e3c44b7df6bb6884185c63
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870133"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="df5eb-103">Тип ресурса Регистрикэйстате</span><span class="sxs-lookup"><span data-stu-id="df5eb-103">registryKeyState resource type</span></span>

<span data-ttu-id="df5eb-104">Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="df5eb-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="df5eb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="df5eb-105">Properties</span></span>

| <span data-ttu-id="df5eb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="df5eb-106">Property</span></span>     | <span data-ttu-id="df5eb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="df5eb-107">Type</span></span>        | <span data-ttu-id="df5eb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df5eb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df5eb-109">семейства</span><span class="sxs-lookup"><span data-stu-id="df5eb-109">hive</span></span>|<span data-ttu-id="df5eb-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="df5eb-110">registryHive</span></span>|<span data-ttu-id="df5eb-111">[Куст реестра Windows](/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="df5eb-111">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="df5eb-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="df5eb-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="df5eb-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="df5eb-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="df5eb-114">HKEY_LOCAL_MACHINE \САМ</span><span class="sxs-lookup"><span data-stu-id="df5eb-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="df5eb-115">HKEY_LOCAL_MACHINE \Секурити</span><span class="sxs-lookup"><span data-stu-id="df5eb-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="df5eb-116">HKEY_LOCAL_MACHINE \Софтваре</span><span class="sxs-lookup"><span data-stu-id="df5eb-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="df5eb-117">HKEY_LOCAL_MACHINE \Систем</span><span class="sxs-lookup"><span data-stu-id="df5eb-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="df5eb-118">HKEY_USERS\\. Умолчани.</span><span class="sxs-lookup"><span data-stu-id="df5eb-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="df5eb-119">Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="df5eb-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="df5eb-120">ключа</span><span class="sxs-lookup"><span data-stu-id="df5eb-120">key</span></span>|<span data-ttu-id="df5eb-121">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-121">String</span></span>|<span data-ttu-id="df5eb-122">Текущий (то есть измененный) раздел реестра (исключая КУСТ).</span><span class="sxs-lookup"><span data-stu-id="df5eb-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="df5eb-123">олдкэй</span><span class="sxs-lookup"><span data-stu-id="df5eb-123">oldKey</span></span>|<span data-ttu-id="df5eb-124">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-124">String</span></span>|<span data-ttu-id="df5eb-125">Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).</span><span class="sxs-lookup"><span data-stu-id="df5eb-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="df5eb-126">олдвалуедата</span><span class="sxs-lookup"><span data-stu-id="df5eb-126">oldValueData</span></span>|<span data-ttu-id="df5eb-127">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-127">String</span></span>|<span data-ttu-id="df5eb-128">Previous (то есть перед изменением) значение раздела реестра (Content).</span><span class="sxs-lookup"><span data-stu-id="df5eb-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="df5eb-129">олдвалуенаме</span><span class="sxs-lookup"><span data-stu-id="df5eb-129">oldValueName</span></span>|<span data-ttu-id="df5eb-130">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-130">String</span></span>|<span data-ttu-id="df5eb-131">Previous (то есть перед изменением) имя значения раздела реестра.</span><span class="sxs-lookup"><span data-stu-id="df5eb-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="df5eb-132">восстановление</span><span class="sxs-lookup"><span data-stu-id="df5eb-132">operation</span></span>|<span data-ttu-id="df5eb-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="df5eb-133">registryOperation</span></span>|<span data-ttu-id="df5eb-134">Операция, в которой изменилось имя и/или значение раздела реестра.</span><span class="sxs-lookup"><span data-stu-id="df5eb-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="df5eb-135">Возможные значения: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="df5eb-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="df5eb-136">processId</span><span class="sxs-lookup"><span data-stu-id="df5eb-136">processId</span></span>|<span data-ttu-id="df5eb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="df5eb-137">Int32</span></span>|<span data-ttu-id="df5eb-138">Идентификатор процесса (PID), который изменил раздел реестра (сведения о процессе будут отображаться в коллекции предупреждений "процессы").</span><span class="sxs-lookup"><span data-stu-id="df5eb-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="df5eb-139">валуедата</span><span class="sxs-lookup"><span data-stu-id="df5eb-139">valueData</span></span>|<span data-ttu-id="df5eb-140">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-140">String</span></span>|<span data-ttu-id="df5eb-141">Текущие (то есть измененные) данные значения раздела реестра (содержимое).</span><span class="sxs-lookup"><span data-stu-id="df5eb-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="df5eb-142">valueName</span><span class="sxs-lookup"><span data-stu-id="df5eb-142">valueName</span></span>|<span data-ttu-id="df5eb-143">String</span><span class="sxs-lookup"><span data-stu-id="df5eb-143">String</span></span>|<span data-ttu-id="df5eb-144">Current (то есть изменено) имя значения раздела реестра</span><span class="sxs-lookup"><span data-stu-id="df5eb-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="df5eb-145">Типом</span><span class="sxs-lookup"><span data-stu-id="df5eb-145">valueType</span></span>|<span data-ttu-id="df5eb-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="df5eb-146">registryValueType</span></span>|[<span data-ttu-id="df5eb-147">Тип значения раздела реестра</span><span class="sxs-lookup"><span data-stu-id="df5eb-147">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="df5eb-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="df5eb-148">REG_BINARY</span></span></li> <li><span data-ttu-id="df5eb-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="df5eb-149">REG_DWORD</span></span></li> <li><span data-ttu-id="df5eb-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="df5eb-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="df5eb-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="df5eb-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="df5eb-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="df5eb-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="df5eb-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="df5eb-153">REG_LINK</span></span></li> <li><span data-ttu-id="df5eb-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="df5eb-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="df5eb-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="df5eb-155">REG_NONE</span></span></li> <li><span data-ttu-id="df5eb-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="df5eb-156">REG_QWORD</span></span></li> <li><span data-ttu-id="df5eb-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="df5eb-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="df5eb-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="df5eb-158">REG_SZ</span></span></li></ul> <span data-ttu-id="df5eb-159">Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="df5eb-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df5eb-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df5eb-160">JSON representation</span></span>

<span data-ttu-id="df5eb-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df5eb-161">The following is a JSON representation of the resource.</span></span>

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
