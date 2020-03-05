---
title: Тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f7826f23746c5579212ef1ba4dc67f22d299272
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490562"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="fa014-103">Тип ресурса win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="fa014-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

<span data-ttu-id="fa014-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa014-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa014-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa014-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa014-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa014-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa014-107">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="fa014-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="fa014-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="fa014-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa014-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa014-109">Properties</span></span>
|<span data-ttu-id="fa014-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa014-110">Property</span></span>|<span data-ttu-id="fa014-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fa014-111">Type</span></span>|<span data-ttu-id="fa014-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fa014-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa014-113">operator</span><span class="sxs-lookup"><span data-stu-id="fa014-113">operator</span></span>|[<span data-ttu-id="fa014-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="fa014-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="fa014-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="fa014-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="fa014-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="fa014-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="fa014-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="fa014-117">detectionValue</span></span>|<span data-ttu-id="fa014-118">String</span><span class="sxs-lookup"><span data-stu-id="fa014-118">String</span></span>|<span data-ttu-id="fa014-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="fa014-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="fa014-120">displayName</span><span class="sxs-lookup"><span data-stu-id="fa014-120">displayName</span></span>|<span data-ttu-id="fa014-121">String</span><span class="sxs-lookup"><span data-stu-id="fa014-121">String</span></span>|<span data-ttu-id="fa014-122">Уникальное отображаемое имя для этого правила</span><span class="sxs-lookup"><span data-stu-id="fa014-122">The unique display name for this rule</span></span>|
|<span data-ttu-id="fa014-123">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="fa014-123">enforceSignatureCheck</span></span>|<span data-ttu-id="fa014-124">Логический</span><span class="sxs-lookup"><span data-stu-id="fa014-124">Boolean</span></span>|<span data-ttu-id="fa014-125">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="fa014-125">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="fa014-126">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="fa014-126">runAs32Bit</span></span>|<span data-ttu-id="fa014-127">Логический</span><span class="sxs-lookup"><span data-stu-id="fa014-127">Boolean</span></span>|<span data-ttu-id="fa014-128">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="fa014-128">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="fa014-129">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="fa014-129">runAsAccount</span></span>|[<span data-ttu-id="fa014-130">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="fa014-130">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="fa014-131">Указывает тип контекста выполнения, в котором выполняется скрипт.</span><span class="sxs-lookup"><span data-stu-id="fa014-131">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="fa014-132">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="fa014-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="fa014-133">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="fa014-133">scriptContent</span></span>|<span data-ttu-id="fa014-134">String</span><span class="sxs-lookup"><span data-stu-id="fa014-134">String</span></span>|<span data-ttu-id="fa014-135">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="fa014-135">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="fa014-136">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="fa014-136">detectionType</span></span>|[<span data-ttu-id="fa014-137">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="fa014-137">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="fa014-138">Тип обнаружения для вывода сценария.</span><span class="sxs-lookup"><span data-stu-id="fa014-138">The detection type for script output.</span></span> <span data-ttu-id="fa014-139">Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="fa014-139">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa014-140">Связи</span><span class="sxs-lookup"><span data-stu-id="fa014-140">Relationships</span></span>
<span data-ttu-id="fa014-141">Нет</span><span class="sxs-lookup"><span data-stu-id="fa014-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa014-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa014-142">JSON Representation</span></span>
<span data-ttu-id="fa014-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa014-143">Here is a JSON representation of the resource.</span></span>
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



