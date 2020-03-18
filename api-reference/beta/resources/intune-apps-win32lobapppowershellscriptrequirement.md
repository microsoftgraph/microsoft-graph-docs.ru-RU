---
title: Тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef7eaa00605214b10438b8c28ba3752903d26bc7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797600"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="7e644-103">Тип ресурса win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="7e644-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

> <span data-ttu-id="7e644-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e644-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e644-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="7e644-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="7e644-107">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="7e644-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e644-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e644-108">Properties</span></span>
|<span data-ttu-id="7e644-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e644-109">Property</span></span>|<span data-ttu-id="7e644-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7e644-110">Type</span></span>|<span data-ttu-id="7e644-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7e644-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e644-112">operator</span><span class="sxs-lookup"><span data-stu-id="7e644-112">operator</span></span>|[<span data-ttu-id="7e644-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="7e644-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="7e644-114">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="7e644-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="7e644-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="7e644-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7e644-116">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="7e644-116">detectionValue</span></span>|<span data-ttu-id="7e644-117">String</span><span class="sxs-lookup"><span data-stu-id="7e644-117">String</span></span>|<span data-ttu-id="7e644-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="7e644-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="7e644-119">displayName</span><span class="sxs-lookup"><span data-stu-id="7e644-119">displayName</span></span>|<span data-ttu-id="7e644-120">String</span><span class="sxs-lookup"><span data-stu-id="7e644-120">String</span></span>|<span data-ttu-id="7e644-121">Уникальное отображаемое имя для этого правила</span><span class="sxs-lookup"><span data-stu-id="7e644-121">The unique display name for this rule</span></span>|
|<span data-ttu-id="7e644-122">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="7e644-122">enforceSignatureCheck</span></span>|<span data-ttu-id="7e644-123">Логический</span><span class="sxs-lookup"><span data-stu-id="7e644-123">Boolean</span></span>|<span data-ttu-id="7e644-124">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="7e644-124">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="7e644-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="7e644-125">runAs32Bit</span></span>|<span data-ttu-id="7e644-126">Логический</span><span class="sxs-lookup"><span data-stu-id="7e644-126">Boolean</span></span>|<span data-ttu-id="7e644-127">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="7e644-127">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="7e644-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="7e644-128">runAsAccount</span></span>|[<span data-ttu-id="7e644-129">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="7e644-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="7e644-130">Указывает тип контекста выполнения, в котором выполняется скрипт.</span><span class="sxs-lookup"><span data-stu-id="7e644-130">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="7e644-131">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="7e644-131">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="7e644-132">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="7e644-132">scriptContent</span></span>|<span data-ttu-id="7e644-133">String</span><span class="sxs-lookup"><span data-stu-id="7e644-133">String</span></span>|<span data-ttu-id="7e644-134">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="7e644-134">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="7e644-135">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="7e644-135">detectionType</span></span>|[<span data-ttu-id="7e644-136">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="7e644-136">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="7e644-137">Тип обнаружения для вывода сценария.</span><span class="sxs-lookup"><span data-stu-id="7e644-137">The detection type for script output.</span></span> <span data-ttu-id="7e644-138">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="7e644-138">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e644-139">Связи</span><span class="sxs-lookup"><span data-stu-id="7e644-139">Relationships</span></span>
<span data-ttu-id="7e644-140">Нет</span><span class="sxs-lookup"><span data-stu-id="7e644-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e644-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e644-141">JSON Representation</span></span>
<span data-ttu-id="7e644-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e644-142">Here is a JSON representation of the resource.</span></span>
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



