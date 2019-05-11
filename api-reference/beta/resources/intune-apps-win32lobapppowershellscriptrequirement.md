---
title: Тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2df6d406f5bc86b2637d60098a819138195b1383
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949516"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="b95aa-103">Тип ресурса win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="b95aa-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

> <span data-ttu-id="b95aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b95aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b95aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b95aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b95aa-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b95aa-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="b95aa-107">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b95aa-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b95aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b95aa-108">Properties</span></span>
|<span data-ttu-id="b95aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b95aa-109">Property</span></span>|<span data-ttu-id="b95aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b95aa-110">Type</span></span>|<span data-ttu-id="b95aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b95aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b95aa-112">operator</span><span class="sxs-lookup"><span data-stu-id="b95aa-112">operator</span></span>|[<span data-ttu-id="b95aa-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="b95aa-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="b95aa-114">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="b95aa-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="b95aa-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="b95aa-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="b95aa-116">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="b95aa-116">detectionValue</span></span>|<span data-ttu-id="b95aa-117">Строка</span><span class="sxs-lookup"><span data-stu-id="b95aa-117">String</span></span>|<span data-ttu-id="b95aa-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b95aa-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="b95aa-119">displayName</span><span class="sxs-lookup"><span data-stu-id="b95aa-119">displayName</span></span>|<span data-ttu-id="b95aa-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b95aa-120">String</span></span>|<span data-ttu-id="b95aa-121">Уникальное отображаемое имя для этого правила</span><span class="sxs-lookup"><span data-stu-id="b95aa-121">The unique display name for this rule</span></span>|
|<span data-ttu-id="b95aa-122">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="b95aa-122">enforceSignatureCheck</span></span>|<span data-ttu-id="b95aa-123">Логический</span><span class="sxs-lookup"><span data-stu-id="b95aa-123">Boolean</span></span>|<span data-ttu-id="b95aa-124">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="b95aa-124">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="b95aa-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="b95aa-125">runAs32Bit</span></span>|<span data-ttu-id="b95aa-126">Логический</span><span class="sxs-lookup"><span data-stu-id="b95aa-126">Boolean</span></span>|<span data-ttu-id="b95aa-127">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="b95aa-127">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="b95aa-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="b95aa-128">runAsAccount</span></span>|[<span data-ttu-id="b95aa-129">Рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="b95aa-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="b95aa-130">Указывает тип контекста выполнения, в котором выполняется скрипт.</span><span class="sxs-lookup"><span data-stu-id="b95aa-130">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="b95aa-131">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b95aa-131">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="b95aa-132">Скриптконтент</span><span class="sxs-lookup"><span data-stu-id="b95aa-132">scriptContent</span></span>|<span data-ttu-id="b95aa-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b95aa-133">String</span></span>|<span data-ttu-id="b95aa-134">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b95aa-134">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="b95aa-135">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="b95aa-135">detectionType</span></span>|[<span data-ttu-id="b95aa-136">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="b95aa-136">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="b95aa-137">Тип обнаружения для вывода сценария.</span><span class="sxs-lookup"><span data-stu-id="b95aa-137">The detection type for script output.</span></span> <span data-ttu-id="b95aa-138">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="b95aa-138">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b95aa-139">Связи</span><span class="sxs-lookup"><span data-stu-id="b95aa-139">Relationships</span></span>
<span data-ttu-id="b95aa-140">Нет</span><span class="sxs-lookup"><span data-stu-id="b95aa-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b95aa-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b95aa-141">JSON Representation</span></span>
<span data-ttu-id="b95aa-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b95aa-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```




