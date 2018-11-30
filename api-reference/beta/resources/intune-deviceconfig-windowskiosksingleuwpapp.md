---
title: Тип ресурса windowsKioskSingleUWPApp
description: Класс, используемый для идентификации информация приложения UWP для базовой конфигурации
ms.openlocfilehash: 009d53d1439894b59a89a1f269df34c4dbb09ce1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079777"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="f4dd6-103">Тип ресурса windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="f4dd6-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="f4dd6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f4dd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4dd6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4dd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4dd6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4dd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4dd6-107">Класс, используемый для идентификации информация приложения UWP для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="f4dd6-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="f4dd6-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4dd6-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4dd6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4dd6-109">Properties</span></span>
|<span data-ttu-id="f4dd6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4dd6-110">Property</span></span>|<span data-ttu-id="f4dd6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f4dd6-111">Type</span></span>|<span data-ttu-id="f4dd6-112">Description</span><span class="sxs-lookup"><span data-stu-id="f4dd6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4dd6-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="f4dd6-113">uwpApp</span></span>|<span data-ttu-id="f4dd6-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="f4dd6-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="f4dd6-115">Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска</span><span class="sxs-lookup"><span data-stu-id="f4dd6-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4dd6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f4dd6-116">Relationships</span></span>
<span data-ttu-id="f4dd6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f4dd6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f4dd6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4dd6-118">JSON Representation</span></span>
<span data-ttu-id="f4dd6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4dd6-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





