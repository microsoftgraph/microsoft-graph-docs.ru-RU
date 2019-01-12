---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства сценария PowerShell для обнаружения приложений Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38a3df87ca5492b89000fc1090395d94c64e1888
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926969"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="f61bd-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="f61bd-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="f61bd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f61bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f61bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f61bd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f61bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f61bd-107">Содержит свойства сценария PowerShell для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="f61bd-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="f61bd-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="f61bd-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f61bd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f61bd-109">Properties</span></span>
|<span data-ttu-id="f61bd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f61bd-110">Property</span></span>|<span data-ttu-id="f61bd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f61bd-111">Type</span></span>|<span data-ttu-id="f61bd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f61bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f61bd-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="f61bd-113">enforceSignatureCheck</span></span>|<span data-ttu-id="f61bd-114">Логический</span><span class="sxs-lookup"><span data-stu-id="f61bd-114">Boolean</span></span>|<span data-ttu-id="f61bd-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="f61bd-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="f61bd-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="f61bd-116">runAs32Bit</span></span>|<span data-ttu-id="f61bd-117">Логический</span><span class="sxs-lookup"><span data-stu-id="f61bd-117">Boolean</span></span>|<span data-ttu-id="f61bd-118">Значение, указывающее, будет ли этот скрипт должна запускаться в 32-разрядная версия</span><span class="sxs-lookup"><span data-stu-id="f61bd-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="f61bd-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f61bd-119">scriptContent</span></span>|<span data-ttu-id="f61bd-120">Строка</span><span class="sxs-lookup"><span data-stu-id="f61bd-120">String</span></span>|<span data-ttu-id="f61bd-121">Содержимое сценария для обнаружения Win32 строки из бизнес-приложения в кодировке base64</span><span class="sxs-lookup"><span data-stu-id="f61bd-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f61bd-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f61bd-122">Relationships</span></span>
<span data-ttu-id="f61bd-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f61bd-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f61bd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f61bd-124">JSON Representation</span></span>
<span data-ttu-id="f61bd-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f61bd-125">Here is a JSON representation of the resource.</span></span>
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





