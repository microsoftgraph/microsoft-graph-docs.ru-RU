---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cc28f3344bf22e263623c068ae93008a20db557
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987329"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="90ca9-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="90ca9-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="90ca9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ca9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ca9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90ca9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ca9-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="90ca9-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="90ca9-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="90ca9-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90ca9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="90ca9-108">Properties</span></span>
|<span data-ttu-id="90ca9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ca9-109">Property</span></span>|<span data-ttu-id="90ca9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="90ca9-110">Type</span></span>|<span data-ttu-id="90ca9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="90ca9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ca9-112">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="90ca9-112">enforceSignatureCheck</span></span>|<span data-ttu-id="90ca9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ca9-113">Boolean</span></span>|<span data-ttu-id="90ca9-114">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="90ca9-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="90ca9-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="90ca9-115">runAs32Bit</span></span>|<span data-ttu-id="90ca9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ca9-116">Boolean</span></span>|<span data-ttu-id="90ca9-117">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="90ca9-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="90ca9-118">Скриптконтент</span><span class="sxs-lookup"><span data-stu-id="90ca9-118">scriptContent</span></span>|<span data-ttu-id="90ca9-119">String</span><span class="sxs-lookup"><span data-stu-id="90ca9-119">String</span></span>|<span data-ttu-id="90ca9-120">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="90ca9-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ca9-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="90ca9-121">Relationships</span></span>
<span data-ttu-id="90ca9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="90ca9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90ca9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90ca9-123">JSON Representation</span></span>
<span data-ttu-id="90ca9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ca9-124">Here is a JSON representation of the resource.</span></span>
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





