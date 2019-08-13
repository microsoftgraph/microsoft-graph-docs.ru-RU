---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5e55629f3d8b17c76eef90711bbff184551fd4b5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335608"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="8f0f0-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="8f0f0-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="8f0f0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f0f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f0f0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f0f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f0f0-106">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="8f0f0-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="8f0f0-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8f0f0-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f0f0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f0f0-108">Properties</span></span>
|<span data-ttu-id="8f0f0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f0f0-109">Property</span></span>|<span data-ttu-id="8f0f0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8f0f0-110">Type</span></span>|<span data-ttu-id="8f0f0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f0f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f0f0-112">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="8f0f0-112">enforceSignatureCheck</span></span>|<span data-ttu-id="8f0f0-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f0f0-113">Boolean</span></span>|<span data-ttu-id="8f0f0-114">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="8f0f0-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="8f0f0-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8f0f0-115">runAs32Bit</span></span>|<span data-ttu-id="8f0f0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f0f0-116">Boolean</span></span>|<span data-ttu-id="8f0f0-117">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="8f0f0-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="8f0f0-118">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="8f0f0-118">scriptContent</span></span>|<span data-ttu-id="8f0f0-119">String</span><span class="sxs-lookup"><span data-stu-id="8f0f0-119">String</span></span>|<span data-ttu-id="8f0f0-120">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="8f0f0-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f0f0-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="8f0f0-121">Relationships</span></span>
<span data-ttu-id="8f0f0-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8f0f0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f0f0-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f0f0-123">JSON Representation</span></span>
<span data-ttu-id="8f0f0-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f0f0-124">Here is a JSON representation of the resource.</span></span>
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



