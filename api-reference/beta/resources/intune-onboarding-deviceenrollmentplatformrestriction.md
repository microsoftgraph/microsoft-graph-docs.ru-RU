---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bf4748d8dc083fe03b55b5ee88062ebb429f639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422861"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4e3cd-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4e3cd-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4e3cd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e3cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e3cd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e3cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e3cd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e3cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3cd-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="4e3cd-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="4e3cd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e3cd-108">Properties</span></span>
|<span data-ttu-id="4e3cd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e3cd-109">Property</span></span>|<span data-ttu-id="4e3cd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4e3cd-110">Type</span></span>|<span data-ttu-id="4e3cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4e3cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3cd-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4e3cd-112">platformBlocked</span></span>|<span data-ttu-id="4e3cd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e3cd-113">Boolean</span></span>|<span data-ttu-id="4e3cd-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="4e3cd-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4e3cd-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4e3cd-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4e3cd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e3cd-116">Boolean</span></span>|<span data-ttu-id="4e3cd-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="4e3cd-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4e3cd-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4e3cd-118">osMinimumVersion</span></span>|<span data-ttu-id="4e3cd-119">String</span><span class="sxs-lookup"><span data-stu-id="4e3cd-119">String</span></span>|<span data-ttu-id="4e3cd-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="4e3cd-120">Min OS version supported</span></span>|
|<span data-ttu-id="4e3cd-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4e3cd-121">osMaximumVersion</span></span>|<span data-ttu-id="4e3cd-122">String</span><span class="sxs-lookup"><span data-stu-id="4e3cd-122">String</span></span>|<span data-ttu-id="4e3cd-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="4e3cd-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e3cd-124">Связи</span><span class="sxs-lookup"><span data-stu-id="4e3cd-124">Relationships</span></span>
<span data-ttu-id="4e3cd-125">Нет</span><span class="sxs-lookup"><span data-stu-id="4e3cd-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e3cd-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e3cd-126">JSON Representation</span></span>
<span data-ttu-id="4e3cd-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e3cd-127">Here is a JSON representation of the resource.</span></span>
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




