---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: edf64c6aaa2a9745b28543bd3dc3a458b7d8869e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367240"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="36e91-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="36e91-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="36e91-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36e91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36e91-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="36e91-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="36e91-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36e91-106">Properties</span></span>
|<span data-ttu-id="36e91-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36e91-107">Property</span></span>|<span data-ttu-id="36e91-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36e91-108">Type</span></span>|<span data-ttu-id="36e91-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36e91-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36e91-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="36e91-110">platformBlocked</span></span>|<span data-ttu-id="36e91-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="36e91-111">Boolean</span></span>|<span data-ttu-id="36e91-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="36e91-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="36e91-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="36e91-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="36e91-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="36e91-114">Boolean</span></span>|<span data-ttu-id="36e91-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="36e91-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="36e91-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="36e91-116">osMinimumVersion</span></span>|<span data-ttu-id="36e91-117">String</span><span class="sxs-lookup"><span data-stu-id="36e91-117">String</span></span>|<span data-ttu-id="36e91-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="36e91-118">Min OS version supported</span></span>|
|<span data-ttu-id="36e91-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="36e91-119">osMaximumVersion</span></span>|<span data-ttu-id="36e91-120">String</span><span class="sxs-lookup"><span data-stu-id="36e91-120">String</span></span>|<span data-ttu-id="36e91-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="36e91-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="36e91-122">Связи</span><span class="sxs-lookup"><span data-stu-id="36e91-122">Relationships</span></span>
<span data-ttu-id="36e91-123">Нет</span><span class="sxs-lookup"><span data-stu-id="36e91-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36e91-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36e91-124">JSON Representation</span></span>
<span data-ttu-id="36e91-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36e91-125">Here is a JSON representation of the resource.</span></span>
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




