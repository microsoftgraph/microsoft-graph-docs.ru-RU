---
title: Тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25ca86e44b6244e592214459c4ebcfbd0f228231
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020390"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="7525d-103">Тип ресурса win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="7525d-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="7525d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7525d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7525d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7525d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7525d-106">Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="7525d-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="7525d-107">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="7525d-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7525d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7525d-108">Properties</span></span>
|<span data-ttu-id="7525d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7525d-109">Property</span></span>|<span data-ttu-id="7525d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7525d-110">Type</span></span>|<span data-ttu-id="7525d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7525d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7525d-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="7525d-112">ruleType</span></span>|[<span data-ttu-id="7525d-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="7525d-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="7525d-114">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="7525d-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="7525d-115">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="7525d-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="7525d-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="7525d-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="7525d-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7525d-117">displayName</span></span>|<span data-ttu-id="7525d-118">String</span><span class="sxs-lookup"><span data-stu-id="7525d-118">String</span></span>|<span data-ttu-id="7525d-119">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="7525d-119">The display name for the rule.</span></span> <span data-ttu-id="7525d-120">Не указывайте это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7525d-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="7525d-121">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="7525d-121">enforceSignatureCheck</span></span>|<span data-ttu-id="7525d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7525d-122">Boolean</span></span>|<span data-ttu-id="7525d-123">Значение, указывающее, применяется ли проверка подписи.</span><span class="sxs-lookup"><span data-stu-id="7525d-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="7525d-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="7525d-124">runAs32Bit</span></span>|<span data-ttu-id="7525d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7525d-125">Boolean</span></span>|<span data-ttu-id="7525d-126">Значение, указывающее, должен ли скрипт выполняться как 32 бит.</span><span class="sxs-lookup"><span data-stu-id="7525d-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="7525d-127">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="7525d-127">scriptContent</span></span>|<span data-ttu-id="7525d-128">String</span><span class="sxs-lookup"><span data-stu-id="7525d-128">String</span></span>|<span data-ttu-id="7525d-129">Содержимое скрипта в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="7525d-129">The base64-encoded script content.</span></span>|
|<span data-ttu-id="7525d-130">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="7525d-130">operationType</span></span>|[<span data-ttu-id="7525d-131">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="7525d-131">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="7525d-132">Тип операции сравнения выходных данных скрипта.</span><span class="sxs-lookup"><span data-stu-id="7525d-132">The script output comparison operation type.</span></span> <span data-ttu-id="7525d-133">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7525d-133">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="7525d-134">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="7525d-134">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="7525d-135">operator</span><span class="sxs-lookup"><span data-stu-id="7525d-135">operator</span></span>|[<span data-ttu-id="7525d-136">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="7525d-136">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="7525d-137">Оператор вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="7525d-137">The script output operator.</span></span> <span data-ttu-id="7525d-138">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7525d-138">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="7525d-139">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="7525d-139">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7525d-140">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="7525d-140">comparisonValue</span></span>|<span data-ttu-id="7525d-141">String</span><span class="sxs-lookup"><span data-stu-id="7525d-141">String</span></span>|<span data-ttu-id="7525d-142">Значение для сравнения вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="7525d-142">The script output comparison value.</span></span> <span data-ttu-id="7525d-143">Не указывайте значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7525d-143">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7525d-144">Связи</span><span class="sxs-lookup"><span data-stu-id="7525d-144">Relationships</span></span>
<span data-ttu-id="7525d-145">Нет</span><span class="sxs-lookup"><span data-stu-id="7525d-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7525d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7525d-146">JSON Representation</span></span>
<span data-ttu-id="7525d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7525d-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```





