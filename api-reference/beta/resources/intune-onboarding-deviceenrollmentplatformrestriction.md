---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5908d1e1d9d2c7eb902017bffdc533e33486f909
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940416"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="079b7-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="079b7-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="079b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="079b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="079b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="079b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="079b7-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="079b7-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="079b7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="079b7-107">Properties</span></span>
|<span data-ttu-id="079b7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="079b7-108">Property</span></span>|<span data-ttu-id="079b7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="079b7-109">Type</span></span>|<span data-ttu-id="079b7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="079b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="079b7-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="079b7-111">platformBlocked</span></span>|<span data-ttu-id="079b7-112">Логический</span><span class="sxs-lookup"><span data-stu-id="079b7-112">Boolean</span></span>|<span data-ttu-id="079b7-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="079b7-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="079b7-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="079b7-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="079b7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="079b7-115">Boolean</span></span>|<span data-ttu-id="079b7-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="079b7-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="079b7-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="079b7-117">osMinimumVersion</span></span>|<span data-ttu-id="079b7-118">Строка</span><span class="sxs-lookup"><span data-stu-id="079b7-118">String</span></span>|<span data-ttu-id="079b7-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="079b7-119">Min OS version supported</span></span>|
|<span data-ttu-id="079b7-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="079b7-120">osMaximumVersion</span></span>|<span data-ttu-id="079b7-121">String</span><span class="sxs-lookup"><span data-stu-id="079b7-121">String</span></span>|<span data-ttu-id="079b7-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="079b7-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="079b7-123">Связи</span><span class="sxs-lookup"><span data-stu-id="079b7-123">Relationships</span></span>
<span data-ttu-id="079b7-124">Нет</span><span class="sxs-lookup"><span data-stu-id="079b7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="079b7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="079b7-125">JSON Representation</span></span>
<span data-ttu-id="079b7-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="079b7-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```




