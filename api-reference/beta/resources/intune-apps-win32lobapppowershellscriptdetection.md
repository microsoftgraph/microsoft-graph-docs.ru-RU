---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства сценария PowerShell для обнаружения приложений Win32
ms.openlocfilehash: e5d87d3d2a90c0ac7f8ce6db7e14b105583a76f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078625"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="94ea5-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="94ea5-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="94ea5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94ea5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94ea5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94ea5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94ea5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="94ea5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94ea5-107">Содержит свойства сценария PowerShell для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="94ea5-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="94ea5-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="94ea5-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94ea5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="94ea5-109">Properties</span></span>
|<span data-ttu-id="94ea5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="94ea5-110">Property</span></span>|<span data-ttu-id="94ea5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="94ea5-111">Type</span></span>|<span data-ttu-id="94ea5-112">Description</span><span class="sxs-lookup"><span data-stu-id="94ea5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94ea5-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="94ea5-113">enforceSignatureCheck</span></span>|<span data-ttu-id="94ea5-114">Логический</span><span class="sxs-lookup"><span data-stu-id="94ea5-114">Boolean</span></span>|<span data-ttu-id="94ea5-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="94ea5-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="94ea5-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="94ea5-116">runAs32Bit</span></span>|<span data-ttu-id="94ea5-117">Логический</span><span class="sxs-lookup"><span data-stu-id="94ea5-117">Boolean</span></span>|<span data-ttu-id="94ea5-118">Значение, указывающее, будет ли этот скрипт должна запускаться в 32-разрядная версия</span><span class="sxs-lookup"><span data-stu-id="94ea5-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="94ea5-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="94ea5-119">scriptContent</span></span>|<span data-ttu-id="94ea5-120">String</span><span class="sxs-lookup"><span data-stu-id="94ea5-120">String</span></span>|<span data-ttu-id="94ea5-121">Содержимое сценария для обнаружения Win32 строки из бизнес-приложения в кодировке base64</span><span class="sxs-lookup"><span data-stu-id="94ea5-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="94ea5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="94ea5-122">Relationships</span></span>
<span data-ttu-id="94ea5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="94ea5-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94ea5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94ea5-124">JSON Representation</span></span>
<span data-ttu-id="94ea5-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94ea5-125">Here is a JSON representation of the resource.</span></span>
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





