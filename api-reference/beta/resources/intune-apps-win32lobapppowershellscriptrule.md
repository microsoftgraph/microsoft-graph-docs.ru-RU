---
title: Тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c392d43f6e9836118f1d32320c5e63498226fed9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712066"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="86ed5-103">Тип ресурса win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="86ed5-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="86ed5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ed5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86ed5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ed5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ed5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86ed5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ed5-107">Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="86ed5-107">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="86ed5-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="86ed5-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86ed5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="86ed5-109">Properties</span></span>
|<span data-ttu-id="86ed5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="86ed5-110">Property</span></span>|<span data-ttu-id="86ed5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="86ed5-111">Type</span></span>|<span data-ttu-id="86ed5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="86ed5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ed5-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="86ed5-113">ruleType</span></span>|[<span data-ttu-id="86ed5-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="86ed5-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="86ed5-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="86ed5-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="86ed5-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="86ed5-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="86ed5-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="86ed5-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="86ed5-118">displayName</span><span class="sxs-lookup"><span data-stu-id="86ed5-118">displayName</span></span>|<span data-ttu-id="86ed5-119">Строка</span><span class="sxs-lookup"><span data-stu-id="86ed5-119">String</span></span>|<span data-ttu-id="86ed5-120">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="86ed5-120">The display name for the rule.</span></span> <span data-ttu-id="86ed5-121">Не указывайте это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-121">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="86ed5-122">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="86ed5-122">enforceSignatureCheck</span></span>|<span data-ttu-id="86ed5-123">Логический</span><span class="sxs-lookup"><span data-stu-id="86ed5-123">Boolean</span></span>|<span data-ttu-id="86ed5-124">Значение, указывающее, применяется ли проверка подписи.</span><span class="sxs-lookup"><span data-stu-id="86ed5-124">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="86ed5-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="86ed5-125">runAs32Bit</span></span>|<span data-ttu-id="86ed5-126">Логический</span><span class="sxs-lookup"><span data-stu-id="86ed5-126">Boolean</span></span>|<span data-ttu-id="86ed5-127">Значение, указывающее, должен ли скрипт выполняться как 32 бит.</span><span class="sxs-lookup"><span data-stu-id="86ed5-127">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="86ed5-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="86ed5-128">runAsAccount</span></span>|[<span data-ttu-id="86ed5-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="86ed5-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="86ed5-130">Контекст выполнения скрипта.</span><span class="sxs-lookup"><span data-stu-id="86ed5-130">The execution context of the script.</span></span> <span data-ttu-id="86ed5-131">Не указывайте это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-131">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="86ed5-132">Правила определения скрипта будут выполняться в том же контексте, что и связанный контекст установки приложения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-132">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="86ed5-133">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="86ed5-133">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="86ed5-134">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="86ed5-134">scriptContent</span></span>|<span data-ttu-id="86ed5-135">Строка</span><span class="sxs-lookup"><span data-stu-id="86ed5-135">String</span></span>|<span data-ttu-id="86ed5-136">Содержимое скрипта в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="86ed5-136">The base64-encoded script content.</span></span>|
|<span data-ttu-id="86ed5-137">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="86ed5-137">operationType</span></span>|[<span data-ttu-id="86ed5-138">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="86ed5-138">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="86ed5-139">Тип операции сравнения выходных данных скрипта.</span><span class="sxs-lookup"><span data-stu-id="86ed5-139">The script output comparison operation type.</span></span> <span data-ttu-id="86ed5-140">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-140">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="86ed5-141">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="86ed5-141">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="86ed5-142">operator</span><span class="sxs-lookup"><span data-stu-id="86ed5-142">operator</span></span>|[<span data-ttu-id="86ed5-143">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="86ed5-143">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="86ed5-144">Оператор вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="86ed5-144">The script output operator.</span></span> <span data-ttu-id="86ed5-145">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-145">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="86ed5-146">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="86ed5-146">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="86ed5-147">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="86ed5-147">comparisonValue</span></span>|<span data-ttu-id="86ed5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="86ed5-148">String</span></span>|<span data-ttu-id="86ed5-149">Значение для сравнения вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="86ed5-149">The script output comparison value.</span></span> <span data-ttu-id="86ed5-150">Не указывайте значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="86ed5-150">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86ed5-151">Связи</span><span class="sxs-lookup"><span data-stu-id="86ed5-151">Relationships</span></span>
<span data-ttu-id="86ed5-152">Нет</span><span class="sxs-lookup"><span data-stu-id="86ed5-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86ed5-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86ed5-153">JSON Representation</span></span>
<span data-ttu-id="86ed5-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86ed5-154">Here is a JSON representation of the resource.</span></span>
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
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```





