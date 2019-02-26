---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260839"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="66cd7-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="66cd7-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="66cd7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66cd7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66cd7-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="66cd7-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="66cd7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="66cd7-106">Properties</span></span>
|<span data-ttu-id="66cd7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="66cd7-107">Property</span></span>|<span data-ttu-id="66cd7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="66cd7-108">Type</span></span>|<span data-ttu-id="66cd7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="66cd7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66cd7-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="66cd7-110">platformBlocked</span></span>|<span data-ttu-id="66cd7-111">Логический</span><span class="sxs-lookup"><span data-stu-id="66cd7-111">Boolean</span></span>|<span data-ttu-id="66cd7-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="66cd7-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="66cd7-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="66cd7-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="66cd7-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="66cd7-114">Boolean</span></span>|<span data-ttu-id="66cd7-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="66cd7-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="66cd7-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="66cd7-116">osMinimumVersion</span></span>|<span data-ttu-id="66cd7-117">String</span><span class="sxs-lookup"><span data-stu-id="66cd7-117">String</span></span>|<span data-ttu-id="66cd7-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="66cd7-118">Min OS version supported</span></span>|
|<span data-ttu-id="66cd7-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="66cd7-119">osMaximumVersion</span></span>|<span data-ttu-id="66cd7-120">String</span><span class="sxs-lookup"><span data-stu-id="66cd7-120">String</span></span>|<span data-ttu-id="66cd7-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="66cd7-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="66cd7-122">Связи</span><span class="sxs-lookup"><span data-stu-id="66cd7-122">Relationships</span></span>
<span data-ttu-id="66cd7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="66cd7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66cd7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66cd7-124">JSON Representation</span></span>
<span data-ttu-id="66cd7-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66cd7-125">Here is a JSON representation of the resource.</span></span>
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



