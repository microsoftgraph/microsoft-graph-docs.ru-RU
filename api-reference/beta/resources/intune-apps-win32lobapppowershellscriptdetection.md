---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507b7adfe3a6d69df99063e69c3651848fc70e22
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273965"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="ed0fb-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="ed0fb-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="ed0fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed0fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed0fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed0fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed0fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed0fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed0fb-107">Содержит свойства скрипта PowerShell для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ed0fb-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="ed0fb-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="ed0fb-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed0fb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed0fb-109">Properties</span></span>
|<span data-ttu-id="ed0fb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed0fb-110">Property</span></span>|<span data-ttu-id="ed0fb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ed0fb-111">Type</span></span>|<span data-ttu-id="ed0fb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ed0fb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed0fb-113">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="ed0fb-113">enforceSignatureCheck</span></span>|<span data-ttu-id="ed0fb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed0fb-114">Boolean</span></span>|<span data-ttu-id="ed0fb-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="ed0fb-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="ed0fb-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="ed0fb-116">runAs32Bit</span></span>|<span data-ttu-id="ed0fb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed0fb-117">Boolean</span></span>|<span data-ttu-id="ed0fb-118">Значение, указывающее, должен ли этот скрипт выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="ed0fb-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="ed0fb-119">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="ed0fb-119">scriptContent</span></span>|<span data-ttu-id="ed0fb-120">String</span><span class="sxs-lookup"><span data-stu-id="ed0fb-120">String</span></span>|<span data-ttu-id="ed0fb-121">Содержимое скрипта в кодировке Base64 для обнаружения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ed0fb-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed0fb-122">Связи</span><span class="sxs-lookup"><span data-stu-id="ed0fb-122">Relationships</span></span>
<span data-ttu-id="ed0fb-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ed0fb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed0fb-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed0fb-124">JSON Representation</span></span>
<span data-ttu-id="ed0fb-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed0fb-125">Here is a JSON representation of the resource.</span></span>
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




