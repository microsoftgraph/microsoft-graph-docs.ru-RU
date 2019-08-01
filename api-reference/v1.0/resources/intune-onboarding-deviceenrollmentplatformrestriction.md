---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 380e40f04c21bb4276c859597610fa3af769fd11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037522"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="ffe00-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffe00-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="ffe00-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffe00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffe00-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="ffe00-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="ffe00-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffe00-106">Properties</span></span>
|<span data-ttu-id="ffe00-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffe00-107">Property</span></span>|<span data-ttu-id="ffe00-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ffe00-108">Type</span></span>|<span data-ttu-id="ffe00-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe00-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe00-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe00-110">platformBlocked</span></span>|<span data-ttu-id="ffe00-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe00-111">Boolean</span></span>|<span data-ttu-id="ffe00-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="ffe00-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="ffe00-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe00-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="ffe00-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe00-114">Boolean</span></span>|<span data-ttu-id="ffe00-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="ffe00-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="ffe00-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ffe00-116">osMinimumVersion</span></span>|<span data-ttu-id="ffe00-117">String</span><span class="sxs-lookup"><span data-stu-id="ffe00-117">String</span></span>|<span data-ttu-id="ffe00-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="ffe00-118">Min OS version supported</span></span>|
|<span data-ttu-id="ffe00-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ffe00-119">osMaximumVersion</span></span>|<span data-ttu-id="ffe00-120">String</span><span class="sxs-lookup"><span data-stu-id="ffe00-120">String</span></span>|<span data-ttu-id="ffe00-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="ffe00-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffe00-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="ffe00-122">Relationships</span></span>
<span data-ttu-id="ffe00-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ffe00-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffe00-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffe00-124">JSON Representation</span></span>
<span data-ttu-id="ffe00-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffe00-125">Here is a JSON representation of the resource.</span></span>
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



