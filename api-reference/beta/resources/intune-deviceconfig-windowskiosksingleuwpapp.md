---
title: Тип ресурса windowsKioskSingleUWPApp
description: Класс, используемый для идентификации информация приложения UWP для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409379"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="e562a-103">Тип ресурса windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="e562a-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="e562a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e562a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e562a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e562a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e562a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e562a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e562a-107">Класс, используемый для идентификации информация приложения UWP для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="e562a-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="e562a-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e562a-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e562a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e562a-109">Properties</span></span>
|<span data-ttu-id="e562a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e562a-110">Property</span></span>|<span data-ttu-id="e562a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e562a-111">Type</span></span>|<span data-ttu-id="e562a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e562a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e562a-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="e562a-113">uwpApp</span></span>|<span data-ttu-id="e562a-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="e562a-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="e562a-115">Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска</span><span class="sxs-lookup"><span data-stu-id="e562a-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="e562a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="e562a-116">Relationships</span></span>
<span data-ttu-id="e562a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e562a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e562a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e562a-118">JSON Representation</span></span>
<span data-ttu-id="e562a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e562a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




