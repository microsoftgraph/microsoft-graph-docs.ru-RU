---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d99505990bb19789046521632441c4026a0ee404
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538716"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="daf69-103">Тип ресурса Мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="daf69-103">mobileAppInstallTimeSettings resource type</span></span>

> <span data-ttu-id="daf69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf69-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daf69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf69-106">Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.</span><span class="sxs-lookup"><span data-stu-id="daf69-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="daf69-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="daf69-107">Properties</span></span>
|<span data-ttu-id="daf69-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="daf69-108">Property</span></span>|<span data-ttu-id="daf69-109">Тип</span><span class="sxs-lookup"><span data-stu-id="daf69-109">Type</span></span>|<span data-ttu-id="daf69-110">Описание</span><span class="sxs-lookup"><span data-stu-id="daf69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf69-111">уселокалтиме</span><span class="sxs-lookup"><span data-stu-id="daf69-111">useLocalTime</span></span>|<span data-ttu-id="daf69-112">Логический</span><span class="sxs-lookup"><span data-stu-id="daf69-112">Boolean</span></span>|<span data-ttu-id="daf69-113">Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="daf69-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="daf69-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="daf69-114">startDateTime</span></span>|<span data-ttu-id="daf69-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf69-115">DateTimeOffset</span></span>|<span data-ttu-id="daf69-116">Время, когда приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="daf69-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="daf69-117">деадлинедатетиме</span><span class="sxs-lookup"><span data-stu-id="daf69-117">deadlineDateTime</span></span>|<span data-ttu-id="daf69-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf69-118">DateTimeOffset</span></span>|<span data-ttu-id="daf69-119">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="daf69-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf69-120">Связи</span><span class="sxs-lookup"><span data-stu-id="daf69-120">Relationships</span></span>
<span data-ttu-id="daf69-121">Нет</span><span class="sxs-lookup"><span data-stu-id="daf69-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="daf69-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daf69-122">JSON Representation</span></span>
<span data-ttu-id="daf69-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daf69-123">Here is a JSON representation of the resource.</span></span>
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



