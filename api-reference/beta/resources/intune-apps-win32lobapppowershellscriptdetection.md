---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5efcfdc14c2c32b51db04a93da4aff5730106219
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797614"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="046ff-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="046ff-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="046ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="046ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="046ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="046ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="046ff-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="046ff-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="046ff-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="046ff-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="046ff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="046ff-108">Properties</span></span>
|<span data-ttu-id="046ff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="046ff-109">Property</span></span>|<span data-ttu-id="046ff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="046ff-110">Type</span></span>|<span data-ttu-id="046ff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="046ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="046ff-112">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="046ff-112">enforceSignatureCheck</span></span>|<span data-ttu-id="046ff-113">Логический</span><span class="sxs-lookup"><span data-stu-id="046ff-113">Boolean</span></span>|<span data-ttu-id="046ff-114">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="046ff-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="046ff-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="046ff-115">runAs32Bit</span></span>|<span data-ttu-id="046ff-116">Логический</span><span class="sxs-lookup"><span data-stu-id="046ff-116">Boolean</span></span>|<span data-ttu-id="046ff-117">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="046ff-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="046ff-118">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="046ff-118">scriptContent</span></span>|<span data-ttu-id="046ff-119">String</span><span class="sxs-lookup"><span data-stu-id="046ff-119">String</span></span>|<span data-ttu-id="046ff-120">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="046ff-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="046ff-121">Связи</span><span class="sxs-lookup"><span data-stu-id="046ff-121">Relationships</span></span>
<span data-ttu-id="046ff-122">Нет</span><span class="sxs-lookup"><span data-stu-id="046ff-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="046ff-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="046ff-123">JSON Representation</span></span>
<span data-ttu-id="046ff-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="046ff-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```



