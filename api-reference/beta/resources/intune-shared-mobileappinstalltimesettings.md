---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 413d37ef0f672289e68e7dd8d8e2d0b6bc7d17ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768508"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="6a6c0-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="6a6c0-103">mobileAppInstallTimeSettings resource type</span></span>

> <span data-ttu-id="6a6c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a6c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a6c0-106">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="6a6c0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a6c0-107">Properties</span></span>
|<span data-ttu-id="6a6c0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a6c0-108">Property</span></span>|<span data-ttu-id="6a6c0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6c0-109">Type</span></span>|<span data-ttu-id="6a6c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a6c0-111">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="6a6c0-111">useLocalTime</span></span>|<span data-ttu-id="6a6c0-112">Логический</span><span class="sxs-lookup"><span data-stu-id="6a6c0-112">Boolean</span></span>|<span data-ttu-id="6a6c0-113">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="6a6c0-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a6c0-114">startDateTime</span></span>|<span data-ttu-id="6a6c0-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a6c0-115">DateTimeOffset</span></span>|<span data-ttu-id="6a6c0-116">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="6a6c0-117">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="6a6c0-117">deadlineDateTime</span></span>|<span data-ttu-id="6a6c0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a6c0-118">DateTimeOffset</span></span>|<span data-ttu-id="6a6c0-119">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a6c0-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6a6c0-120">Relationships</span></span>
<span data-ttu-id="6a6c0-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6a6c0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a6c0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a6c0-122">JSON Representation</span></span>
<span data-ttu-id="6a6c0-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a6c0-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```



