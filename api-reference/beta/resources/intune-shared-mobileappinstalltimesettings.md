---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 904fc60d28ce8fcca52ea8b84c81d99031ed9ee7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466131"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="6b644-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="6b644-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="6b644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b644-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b644-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b644-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b644-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b644-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b644-107">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="6b644-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="6b644-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b644-108">Properties</span></span>
|<span data-ttu-id="6b644-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b644-109">Property</span></span>|<span data-ttu-id="6b644-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6b644-110">Type</span></span>|<span data-ttu-id="6b644-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b644-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b644-112">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="6b644-112">useLocalTime</span></span>|<span data-ttu-id="6b644-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b644-113">Boolean</span></span>|<span data-ttu-id="6b644-114">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="6b644-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="6b644-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6b644-115">startDateTime</span></span>|<span data-ttu-id="6b644-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b644-116">DateTimeOffset</span></span>|<span data-ttu-id="6b644-117">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="6b644-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="6b644-118">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="6b644-118">deadlineDateTime</span></span>|<span data-ttu-id="6b644-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b644-119">DateTimeOffset</span></span>|<span data-ttu-id="6b644-120">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="6b644-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b644-121">Связи</span><span class="sxs-lookup"><span data-stu-id="6b644-121">Relationships</span></span>
<span data-ttu-id="6b644-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6b644-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b644-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b644-123">JSON Representation</span></span>
<span data-ttu-id="6b644-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b644-124">Here is a JSON representation of the resource.</span></span>
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



