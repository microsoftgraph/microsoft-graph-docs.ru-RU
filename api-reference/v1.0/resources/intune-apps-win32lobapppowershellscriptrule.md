---
title: тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcc9afa8f58462bda69c96990e37529667d20445
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758990"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="58f8b-103">тип ресурса win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="58f8b-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="58f8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58f8b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58f8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58f8b-106">Сложный тип для хранения данных правила скрипта PowerShell для приложения LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="58f8b-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="58f8b-107">Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="58f8b-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58f8b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="58f8b-108">Properties</span></span>
|<span data-ttu-id="58f8b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="58f8b-109">Property</span></span>|<span data-ttu-id="58f8b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="58f8b-110">Type</span></span>|<span data-ttu-id="58f8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="58f8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f8b-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="58f8b-112">ruleType</span></span>|[<span data-ttu-id="58f8b-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="58f8b-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="58f8b-114">Тип правила, указывающий цель правила.</span><span class="sxs-lookup"><span data-stu-id="58f8b-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="58f8b-115">Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="58f8b-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="58f8b-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="58f8b-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="58f8b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="58f8b-117">displayName</span></span>|<span data-ttu-id="58f8b-118">String</span><span class="sxs-lookup"><span data-stu-id="58f8b-118">String</span></span>|<span data-ttu-id="58f8b-119">Имя отображения правила.</span><span class="sxs-lookup"><span data-stu-id="58f8b-119">The display name for the rule.</span></span> <span data-ttu-id="58f8b-120">Не укажите это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="58f8b-121">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="58f8b-121">enforceSignatureCheck</span></span>|<span data-ttu-id="58f8b-122">Логический</span><span class="sxs-lookup"><span data-stu-id="58f8b-122">Boolean</span></span>|<span data-ttu-id="58f8b-123">Значение, указывающее, выполняется ли проверка подписи.</span><span class="sxs-lookup"><span data-stu-id="58f8b-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="58f8b-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="58f8b-124">runAs32Bit</span></span>|<span data-ttu-id="58f8b-125">Логический</span><span class="sxs-lookup"><span data-stu-id="58f8b-125">Boolean</span></span>|<span data-ttu-id="58f8b-126">Значение, указывающее, должен ли скрипт работать как 32-битный.</span><span class="sxs-lookup"><span data-stu-id="58f8b-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="58f8b-127">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="58f8b-127">runAsAccount</span></span>|[<span data-ttu-id="58f8b-128">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="58f8b-128">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="58f8b-129">Контекст выполнения сценария.</span><span class="sxs-lookup"><span data-stu-id="58f8b-129">The execution context of the script.</span></span> <span data-ttu-id="58f8b-130">Не укажите это значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-130">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="58f8b-131">Правила обнаружения скриптов будут работать в том же контексте, что и контекст установки связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-131">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="58f8b-132">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="58f8b-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="58f8b-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="58f8b-133">scriptContent</span></span>|<span data-ttu-id="58f8b-134">String</span><span class="sxs-lookup"><span data-stu-id="58f8b-134">String</span></span>|<span data-ttu-id="58f8b-135">Содержимое скрипта с кодом base64.</span><span class="sxs-lookup"><span data-stu-id="58f8b-135">The base64-encoded script content.</span></span>|
|<span data-ttu-id="58f8b-136">operationType</span><span class="sxs-lookup"><span data-stu-id="58f8b-136">operationType</span></span>|[<span data-ttu-id="58f8b-137">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="58f8b-137">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="58f8b-138">Тип операции сравнения вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="58f8b-138">The script output comparison operation type.</span></span> <span data-ttu-id="58f8b-139">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-139">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="58f8b-140">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="58f8b-140">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="58f8b-141">operator</span><span class="sxs-lookup"><span data-stu-id="58f8b-141">operator</span></span>|[<span data-ttu-id="58f8b-142">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="58f8b-142">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="58f8b-143">Оператор вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="58f8b-143">The script output operator.</span></span> <span data-ttu-id="58f8b-144">Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-144">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="58f8b-145">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="58f8b-145">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="58f8b-146">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="58f8b-146">comparisonValue</span></span>|<span data-ttu-id="58f8b-147">String</span><span class="sxs-lookup"><span data-stu-id="58f8b-147">String</span></span>|<span data-ttu-id="58f8b-148">Значение сравнения вывода скрипта.</span><span class="sxs-lookup"><span data-stu-id="58f8b-148">The script output comparison value.</span></span> <span data-ttu-id="58f8b-149">Не укажите значение, если правило используется для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="58f8b-149">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58f8b-150">Связи</span><span class="sxs-lookup"><span data-stu-id="58f8b-150">Relationships</span></span>
<span data-ttu-id="58f8b-151">Нет</span><span class="sxs-lookup"><span data-stu-id="58f8b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58f8b-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58f8b-152">JSON Representation</span></span>
<span data-ttu-id="58f8b-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58f8b-153">Here is a JSON representation of the resource.</span></span>
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




