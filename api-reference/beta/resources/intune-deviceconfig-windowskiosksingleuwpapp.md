---
title: Тип ресурса windowsKioskSingleUWPApp
description: Класс, используемый для идентификации информация приложения UWP для базовой конфигурации
author: tfitzmac
ms.openlocfilehash: fd1dffd5a01b89db27132770d4c8ffe0094eed8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312182"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="6ba97-103">Тип ресурса windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="6ba97-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="6ba97-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ba97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ba97-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ba97-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ba97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ba97-107">Класс, используемый для идентификации информация приложения UWP для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="6ba97-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="6ba97-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba97-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ba97-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ba97-109">Properties</span></span>
|<span data-ttu-id="6ba97-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ba97-110">Property</span></span>|<span data-ttu-id="6ba97-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6ba97-111">Type</span></span>|<span data-ttu-id="6ba97-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6ba97-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba97-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="6ba97-113">uwpApp</span></span>|<span data-ttu-id="6ba97-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="6ba97-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="6ba97-115">Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска</span><span class="sxs-lookup"><span data-stu-id="6ba97-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ba97-116">Связи</span><span class="sxs-lookup"><span data-stu-id="6ba97-116">Relationships</span></span>
<span data-ttu-id="6ba97-117">Нет</span><span class="sxs-lookup"><span data-stu-id="6ba97-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ba97-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ba97-118">JSON Representation</span></span>
<span data-ttu-id="6ba97-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ba97-119">Here is a JSON representation of the resource.</span></span>
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





