---
title: Тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97f9c8985ffac6dc6f3f736c3b089662d4f2d1ef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422771"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="7211e-103">Тип ресурса win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="7211e-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

<span data-ttu-id="7211e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7211e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7211e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7211e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7211e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7211e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7211e-107">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="7211e-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="7211e-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="7211e-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7211e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7211e-109">Properties</span></span>
|<span data-ttu-id="7211e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7211e-110">Property</span></span>|<span data-ttu-id="7211e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7211e-111">Type</span></span>|<span data-ttu-id="7211e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7211e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7211e-113">operator</span><span class="sxs-lookup"><span data-stu-id="7211e-113">operator</span></span>|[<span data-ttu-id="7211e-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="7211e-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="7211e-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="7211e-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="7211e-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="7211e-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7211e-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="7211e-117">detectionValue</span></span>|<span data-ttu-id="7211e-118">String</span><span class="sxs-lookup"><span data-stu-id="7211e-118">String</span></span>|<span data-ttu-id="7211e-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="7211e-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="7211e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="7211e-120">displayName</span></span>|<span data-ttu-id="7211e-121">String</span><span class="sxs-lookup"><span data-stu-id="7211e-121">String</span></span>|<span data-ttu-id="7211e-122">Уникальное отображаемое имя для этого правила</span><span class="sxs-lookup"><span data-stu-id="7211e-122">The unique display name for this rule</span></span>|
|<span data-ttu-id="7211e-123">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="7211e-123">enforceSignatureCheck</span></span>|<span data-ttu-id="7211e-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7211e-124">Boolean</span></span>|<span data-ttu-id="7211e-125">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="7211e-125">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="7211e-126">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="7211e-126">runAs32Bit</span></span>|<span data-ttu-id="7211e-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7211e-127">Boolean</span></span>|<span data-ttu-id="7211e-128">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="7211e-128">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="7211e-129">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="7211e-129">runAsAccount</span></span>|[<span data-ttu-id="7211e-130">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="7211e-130">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="7211e-131">Указывает тип контекста выполнения, в котором выполняется скрипт.</span><span class="sxs-lookup"><span data-stu-id="7211e-131">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="7211e-132">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="7211e-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="7211e-133">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="7211e-133">scriptContent</span></span>|<span data-ttu-id="7211e-134">String</span><span class="sxs-lookup"><span data-stu-id="7211e-134">String</span></span>|<span data-ttu-id="7211e-135">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="7211e-135">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="7211e-136">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="7211e-136">detectionType</span></span>|[<span data-ttu-id="7211e-137">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="7211e-137">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="7211e-138">Тип обнаружения для вывода сценария.</span><span class="sxs-lookup"><span data-stu-id="7211e-138">The detection type for script output.</span></span> <span data-ttu-id="7211e-139">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="7211e-139">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7211e-140">Связи</span><span class="sxs-lookup"><span data-stu-id="7211e-140">Relationships</span></span>
<span data-ttu-id="7211e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="7211e-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7211e-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7211e-142">JSON Representation</span></span>
<span data-ttu-id="7211e-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7211e-143">Here is a JSON representation of the resource.</span></span>
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



