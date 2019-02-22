---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa5452fd9e73aef846d0b6de86a2b84e2c42ba26
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168525"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="46439-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="46439-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="46439-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46439-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46439-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46439-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46439-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="46439-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="46439-107">НаСледуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="46439-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46439-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="46439-108">Properties</span></span>
|<span data-ttu-id="46439-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="46439-109">Property</span></span>|<span data-ttu-id="46439-110">Тип</span><span class="sxs-lookup"><span data-stu-id="46439-110">Type</span></span>|<span data-ttu-id="46439-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46439-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46439-112">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="46439-112">enforceSignatureCheck</span></span>|<span data-ttu-id="46439-113">Логический</span><span class="sxs-lookup"><span data-stu-id="46439-113">Boolean</span></span>|<span data-ttu-id="46439-114">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="46439-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="46439-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="46439-115">runAs32Bit</span></span>|<span data-ttu-id="46439-116">Логический</span><span class="sxs-lookup"><span data-stu-id="46439-116">Boolean</span></span>|<span data-ttu-id="46439-117">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="46439-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="46439-118">Скриптконтент</span><span class="sxs-lookup"><span data-stu-id="46439-118">scriptContent</span></span>|<span data-ttu-id="46439-119">String</span><span class="sxs-lookup"><span data-stu-id="46439-119">String</span></span>|<span data-ttu-id="46439-120">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="46439-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="46439-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="46439-121">Relationships</span></span>
<span data-ttu-id="46439-122">Нет</span><span class="sxs-lookup"><span data-stu-id="46439-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46439-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46439-123">JSON Representation</span></span>
<span data-ttu-id="46439-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46439-124">Here is a JSON representation of the resource.</span></span>
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




