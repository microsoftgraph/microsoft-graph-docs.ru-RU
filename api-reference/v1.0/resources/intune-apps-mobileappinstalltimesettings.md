---
title: тип ресурса mobileAppInstallTimeSettings
description: Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb768938ffa2e167f13a267451041b65f39011c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755121"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="58418-103">тип ресурса mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="58418-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="58418-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58418-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58418-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58418-106">Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.</span><span class="sxs-lookup"><span data-stu-id="58418-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="58418-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58418-107">Properties</span></span>
|<span data-ttu-id="58418-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="58418-108">Property</span></span>|<span data-ttu-id="58418-109">Тип</span><span class="sxs-lookup"><span data-stu-id="58418-109">Type</span></span>|<span data-ttu-id="58418-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58418-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58418-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="58418-111">useLocalTime</span></span>|<span data-ttu-id="58418-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="58418-112">Boolean</span></span>|<span data-ttu-id="58418-113">Следует ли использовать местное время устройства или время UTC при определении доступных и крайних сроков.</span><span class="sxs-lookup"><span data-stu-id="58418-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="58418-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="58418-114">startDateTime</span></span>|<span data-ttu-id="58418-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58418-115">DateTimeOffset</span></span>|<span data-ttu-id="58418-116">Время, в которое приложение должно быть доступно для установки.</span><span class="sxs-lookup"><span data-stu-id="58418-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="58418-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="58418-117">deadlineDateTime</span></span>|<span data-ttu-id="58418-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58418-118">DateTimeOffset</span></span>|<span data-ttu-id="58418-119">Время установки приложения.</span><span class="sxs-lookup"><span data-stu-id="58418-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58418-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="58418-120">Relationships</span></span>
<span data-ttu-id="58418-121">Нет</span><span class="sxs-lookup"><span data-stu-id="58418-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58418-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58418-122">JSON Representation</span></span>
<span data-ttu-id="58418-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58418-123">Here is a JSON representation of the resource.</span></span>
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




