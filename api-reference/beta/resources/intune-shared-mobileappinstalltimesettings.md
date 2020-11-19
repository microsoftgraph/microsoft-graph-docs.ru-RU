---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8aec3852f68813d6d42acbec73f76c6e32f9ab92
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266132"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="89f06-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="89f06-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="89f06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89f06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89f06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89f06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f06-107">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="89f06-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="89f06-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f06-108">Properties</span></span>
|<span data-ttu-id="89f06-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f06-109">Property</span></span>|<span data-ttu-id="89f06-110">Тип</span><span class="sxs-lookup"><span data-stu-id="89f06-110">Type</span></span>|<span data-ttu-id="89f06-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89f06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f06-112">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="89f06-112">useLocalTime</span></span>|<span data-ttu-id="89f06-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f06-113">Boolean</span></span>|<span data-ttu-id="89f06-114">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="89f06-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="89f06-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="89f06-115">startDateTime</span></span>|<span data-ttu-id="89f06-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f06-116">DateTimeOffset</span></span>|<span data-ttu-id="89f06-117">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="89f06-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="89f06-118">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="89f06-118">deadlineDateTime</span></span>|<span data-ttu-id="89f06-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f06-119">DateTimeOffset</span></span>|<span data-ttu-id="89f06-120">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="89f06-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f06-121">Связи</span><span class="sxs-lookup"><span data-stu-id="89f06-121">Relationships</span></span>
<span data-ttu-id="89f06-122">Нет</span><span class="sxs-lookup"><span data-stu-id="89f06-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f06-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89f06-123">JSON Representation</span></span>
<span data-ttu-id="89f06-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89f06-124">Here is a JSON representation of the resource.</span></span>
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




