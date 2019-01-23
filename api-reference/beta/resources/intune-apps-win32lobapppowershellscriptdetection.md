---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства сценария PowerShell для обнаружения приложений Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399642"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="aff56-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="aff56-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="aff56-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aff56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aff56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aff56-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aff56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff56-107">Содержит свойства сценария PowerShell для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="aff56-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="aff56-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="aff56-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aff56-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff56-109">Properties</span></span>
|<span data-ttu-id="aff56-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff56-110">Property</span></span>|<span data-ttu-id="aff56-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aff56-111">Type</span></span>|<span data-ttu-id="aff56-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aff56-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff56-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="aff56-113">enforceSignatureCheck</span></span>|<span data-ttu-id="aff56-114">Логический</span><span class="sxs-lookup"><span data-stu-id="aff56-114">Boolean</span></span>|<span data-ttu-id="aff56-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="aff56-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="aff56-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="aff56-116">runAs32Bit</span></span>|<span data-ttu-id="aff56-117">Логический</span><span class="sxs-lookup"><span data-stu-id="aff56-117">Boolean</span></span>|<span data-ttu-id="aff56-118">Значение, указывающее, будет ли этот скрипт должна запускаться в 32-разрядная версия</span><span class="sxs-lookup"><span data-stu-id="aff56-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="aff56-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="aff56-119">scriptContent</span></span>|<span data-ttu-id="aff56-120">String</span><span class="sxs-lookup"><span data-stu-id="aff56-120">String</span></span>|<span data-ttu-id="aff56-121">Содержимое сценария для обнаружения Win32 строки из бизнес-приложения в кодировке base64</span><span class="sxs-lookup"><span data-stu-id="aff56-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff56-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="aff56-122">Relationships</span></span>
<span data-ttu-id="aff56-123">Нет</span><span class="sxs-lookup"><span data-stu-id="aff56-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff56-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff56-124">JSON Representation</span></span>
<span data-ttu-id="aff56-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff56-125">Here is a JSON representation of the resource.</span></span>
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




