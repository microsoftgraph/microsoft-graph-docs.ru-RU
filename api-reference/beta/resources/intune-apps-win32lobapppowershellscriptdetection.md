---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 024ef2708dae3a6c4b030b41d86abbd4c21b6d49
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490590"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="0a88a-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="0a88a-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="0a88a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0a88a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a88a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a88a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a88a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a88a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a88a-107">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="0a88a-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="0a88a-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="0a88a-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a88a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a88a-109">Properties</span></span>
|<span data-ttu-id="0a88a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a88a-110">Property</span></span>|<span data-ttu-id="0a88a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0a88a-111">Type</span></span>|<span data-ttu-id="0a88a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0a88a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a88a-113">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="0a88a-113">enforceSignatureCheck</span></span>|<span data-ttu-id="0a88a-114">Логический</span><span class="sxs-lookup"><span data-stu-id="0a88a-114">Boolean</span></span>|<span data-ttu-id="0a88a-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="0a88a-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="0a88a-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0a88a-116">runAs32Bit</span></span>|<span data-ttu-id="0a88a-117">Логический</span><span class="sxs-lookup"><span data-stu-id="0a88a-117">Boolean</span></span>|<span data-ttu-id="0a88a-118">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="0a88a-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="0a88a-119">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="0a88a-119">scriptContent</span></span>|<span data-ttu-id="0a88a-120">String</span><span class="sxs-lookup"><span data-stu-id="0a88a-120">String</span></span>|<span data-ttu-id="0a88a-121">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="0a88a-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a88a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="0a88a-122">Relationships</span></span>
<span data-ttu-id="0a88a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="0a88a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a88a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a88a-124">JSON Representation</span></span>
<span data-ttu-id="0a88a-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a88a-125">Here is a JSON representation of the resource.</span></span>
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



