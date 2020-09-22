---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 77e12b4d22920cccb51aa9a2980f9fc84f95403e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48096063"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="64695-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="64695-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="64695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64695-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64695-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64695-106">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="64695-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="64695-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64695-107">Properties</span></span>
|<span data-ttu-id="64695-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="64695-108">Property</span></span>|<span data-ttu-id="64695-109">Тип</span><span class="sxs-lookup"><span data-stu-id="64695-109">Type</span></span>|<span data-ttu-id="64695-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64695-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64695-111">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="64695-111">useLocalTime</span></span>|<span data-ttu-id="64695-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="64695-112">Boolean</span></span>|<span data-ttu-id="64695-113">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="64695-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="64695-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="64695-114">startDateTime</span></span>|<span data-ttu-id="64695-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64695-115">DateTimeOffset</span></span>|<span data-ttu-id="64695-116">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="64695-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="64695-117">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="64695-117">deadlineDateTime</span></span>|<span data-ttu-id="64695-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64695-118">DateTimeOffset</span></span>|<span data-ttu-id="64695-119">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="64695-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64695-120">Связи</span><span class="sxs-lookup"><span data-stu-id="64695-120">Relationships</span></span>
<span data-ttu-id="64695-121">Нет</span><span class="sxs-lookup"><span data-stu-id="64695-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64695-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64695-122">JSON Representation</span></span>
<span data-ttu-id="64695-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64695-123">Here is a JSON representation of the resource.</span></span>
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





