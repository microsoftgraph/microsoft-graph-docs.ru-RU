---
title: Тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33ebf8bc34996617eece886b02fccf09eabdf504
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790826"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="a08b4-103">Тип ресурса win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="a08b4-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="a08b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a08b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a08b4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a08b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a08b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a08b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a08b4-107">Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="a08b4-107">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="a08b4-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="a08b4-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a08b4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a08b4-109">Properties</span></span>
|<span data-ttu-id="a08b4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a08b4-110">Property</span></span>|<span data-ttu-id="a08b4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a08b4-111">Type</span></span>|<span data-ttu-id="a08b4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a08b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a08b4-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="a08b4-113">ruleType</span></span>|[<span data-ttu-id="a08b4-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="a08b4-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="a08b4-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="a08b4-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="a08b4-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="a08b4-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="a08b4-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="a08b4-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="a08b4-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a08b4-118">displayName</span></span>|<span data-ttu-id="a08b4-119">String</span><span class="sxs-lookup"><span data-stu-id="a08b4-119">String</span></span>|<span data-ttu-id="a08b4-120">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="a08b4-120">The display name for the rule.</span></span> <span data-ttu-id="a08b4-121">Не указывайте это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-121">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="a08b4-122">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="a08b4-122">enforceSignatureCheck</span></span>|<span data-ttu-id="a08b4-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a08b4-123">Boolean</span></span>|<span data-ttu-id="a08b4-124">Значение, указывающее, применяется ли проверка подписи.</span><span class="sxs-lookup"><span data-stu-id="a08b4-124">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="a08b4-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="a08b4-125">runAs32Bit</span></span>|<span data-ttu-id="a08b4-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a08b4-126">Boolean</span></span>|<span data-ttu-id="a08b4-127">Значение, указывающее, должен ли скрипт выполняться как 32 бит.</span><span class="sxs-lookup"><span data-stu-id="a08b4-127">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="a08b4-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="a08b4-128">runAsAccount</span></span>|[<span data-ttu-id="a08b4-129">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="a08b4-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="a08b4-130">Контекст выполнения скрипта.</span><span class="sxs-lookup"><span data-stu-id="a08b4-130">The execution context of the script.</span></span> <span data-ttu-id="a08b4-131">Не указывайте это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-131">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="a08b4-132">Правила определения скрипта будут выполняться в том же контексте, что и связанный контекст установки приложения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-132">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="a08b4-133">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a08b4-133">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="a08b4-134">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="a08b4-134">scriptContent</span></span>|<span data-ttu-id="a08b4-135">String</span><span class="sxs-lookup"><span data-stu-id="a08b4-135">String</span></span>|<span data-ttu-id="a08b4-136">Содержимое скрипта в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="a08b4-136">The base64-encoded script content.</span></span>|
|<span data-ttu-id="a08b4-137">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="a08b4-137">operationType</span></span>|[<span data-ttu-id="a08b4-138">win32LobPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="a08b4-138">win32LobPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobpowershellscriptruleoperationtype.md)|<span data-ttu-id="a08b4-139">Тип операции сравнения выходных данных скрипта.</span><span class="sxs-lookup"><span data-stu-id="a08b4-139">The script output comparison operation type.</span></span> <span data-ttu-id="a08b4-140">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-140">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="a08b4-141">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="a08b4-141">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="a08b4-142">operator</span><span class="sxs-lookup"><span data-stu-id="a08b4-142">operator</span></span>|[<span data-ttu-id="a08b4-143">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="a08b4-143">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="a08b4-144">Оператор вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="a08b4-144">The script output operator.</span></span> <span data-ttu-id="a08b4-145">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-145">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="a08b4-146">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="a08b4-146">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a08b4-147">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="a08b4-147">comparisonValue</span></span>|<span data-ttu-id="a08b4-148">String</span><span class="sxs-lookup"><span data-stu-id="a08b4-148">String</span></span>|<span data-ttu-id="a08b4-149">Значение для сравнения вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="a08b4-149">The script output comparison value.</span></span> <span data-ttu-id="a08b4-150">Не указывайте значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a08b4-150">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a08b4-151">Связи</span><span class="sxs-lookup"><span data-stu-id="a08b4-151">Relationships</span></span>
<span data-ttu-id="a08b4-152">Нет</span><span class="sxs-lookup"><span data-stu-id="a08b4-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a08b4-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a08b4-153">JSON Representation</span></span>
<span data-ttu-id="a08b4-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a08b4-154">Here is a JSON representation of the resource.</span></span>
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



