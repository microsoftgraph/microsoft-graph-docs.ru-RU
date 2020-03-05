---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ff666c29e75d6571dede3834b4660f43e863826
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523620"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="3b860-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="3b860-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="3b860-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b860-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b860-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b860-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b860-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b860-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b860-107">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="3b860-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="3b860-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b860-108">Properties</span></span>
|<span data-ttu-id="3b860-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b860-109">Property</span></span>|<span data-ttu-id="3b860-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3b860-110">Type</span></span>|<span data-ttu-id="3b860-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3b860-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b860-112">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="3b860-112">useLocalTime</span></span>|<span data-ttu-id="3b860-113">Логический</span><span class="sxs-lookup"><span data-stu-id="3b860-113">Boolean</span></span>|<span data-ttu-id="3b860-114">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="3b860-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="3b860-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b860-115">startDateTime</span></span>|<span data-ttu-id="3b860-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b860-116">DateTimeOffset</span></span>|<span data-ttu-id="3b860-117">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="3b860-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="3b860-118">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="3b860-118">deadlineDateTime</span></span>|<span data-ttu-id="3b860-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b860-119">DateTimeOffset</span></span>|<span data-ttu-id="3b860-120">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="3b860-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b860-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3b860-121">Relationships</span></span>
<span data-ttu-id="3b860-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3b860-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b860-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b860-123">JSON Representation</span></span>
<span data-ttu-id="3b860-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b860-124">Here is a JSON representation of the resource.</span></span>
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



