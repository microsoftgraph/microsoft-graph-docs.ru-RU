---
title: тип ресурса windowsKioskSingleWin32App
description: Класс, используемый для определения конфигурации одного приложения для конфигурации киоска win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fefde9fa13849a910c56e4ebaed870ebb9edac62
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447634"
---
# <a name="windowskiosksinglewin32app-resource-type"></a><span data-ttu-id="8814b-103">тип ресурса windowsKioskSingleWin32App</span><span class="sxs-lookup"><span data-stu-id="8814b-103">windowsKioskSingleWin32App resource type</span></span>

<span data-ttu-id="8814b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8814b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8814b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8814b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8814b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8814b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8814b-107">Класс, используемый для определения конфигурации одного приложения для конфигурации киоска win32</span><span class="sxs-lookup"><span data-stu-id="8814b-107">The class used to identify the single app configuration for the kiosk win32 configuration</span></span>


<span data-ttu-id="8814b-108">Наследует [от windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8814b-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8814b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8814b-109">Properties</span></span>
|<span data-ttu-id="8814b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8814b-110">Property</span></span>|<span data-ttu-id="8814b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8814b-111">Type</span></span>|<span data-ttu-id="8814b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8814b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8814b-113">win32App</span><span class="sxs-lookup"><span data-stu-id="8814b-113">win32App</span></span>|[<span data-ttu-id="8814b-114">windowsKioskWin32App</span><span class="sxs-lookup"><span data-stu-id="8814b-114">windowsKioskWin32App</span></span>](../resources/intune-deviceconfig-windowskioskwin32app.md)|<span data-ttu-id="8814b-115">Это приложение win32, которое будет доступно для запуска использования в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="8814b-115">This is the win32 app that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="8814b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8814b-116">Relationships</span></span>
<span data-ttu-id="8814b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8814b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8814b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8814b-118">JSON Representation</span></span>
<span data-ttu-id="8814b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8814b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleWin32App",
  "win32App": {
    "@odata.type": "microsoft.graph.windowsKioskWin32App",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "classicAppPath": "String",
    "edgeNoFirstRun": true,
    "edgeKioskIdleTimeoutMinutes": 1024,
    "edgeKioskType": "String",
    "edgeKiosk": "String"
  }
}
```




