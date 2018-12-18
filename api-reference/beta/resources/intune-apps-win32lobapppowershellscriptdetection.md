---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства сценария PowerShell для обнаружения приложений Win32
author: tfitzmac
ms.openlocfilehash: 7f69b2c066ae90cfcd805b3d3cfe57193046d440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327575"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="2d0b6-103">Тип ресурса win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="2d0b6-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="2d0b6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d0b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d0b6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d0b6-107">Содержит свойства сценария PowerShell для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="2d0b6-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="2d0b6-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="2d0b6-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2d0b6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d0b6-109">Properties</span></span>
|<span data-ttu-id="2d0b6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d0b6-110">Property</span></span>|<span data-ttu-id="2d0b6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2d0b6-111">Type</span></span>|<span data-ttu-id="2d0b6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d0b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d0b6-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="2d0b6-113">enforceSignatureCheck</span></span>|<span data-ttu-id="2d0b6-114">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-114">Boolean</span></span>|<span data-ttu-id="2d0b6-115">Значение, указывающее, применяется ли проверка подписи</span><span class="sxs-lookup"><span data-stu-id="2d0b6-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="2d0b6-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="2d0b6-116">runAs32Bit</span></span>|<span data-ttu-id="2d0b6-117">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-117">Boolean</span></span>|<span data-ttu-id="2d0b6-118">Значение, указывающее, будет ли этот скрипт должна запускаться в 32-разрядная версия</span><span class="sxs-lookup"><span data-stu-id="2d0b6-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="2d0b6-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2d0b6-119">scriptContent</span></span>|<span data-ttu-id="2d0b6-120">String.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-120">String</span></span>|<span data-ttu-id="2d0b6-121">Содержимое сценария для обнаружения Win32 строки из бизнес-приложения в кодировке base64</span><span class="sxs-lookup"><span data-stu-id="2d0b6-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d0b6-122">Связи</span><span class="sxs-lookup"><span data-stu-id="2d0b6-122">Relationships</span></span>
<span data-ttu-id="2d0b6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2d0b6-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d0b6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d0b6-124">JSON Representation</span></span>
<span data-ttu-id="2d0b6-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d0b6-125">Here is a JSON representation of the resource.</span></span>
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





