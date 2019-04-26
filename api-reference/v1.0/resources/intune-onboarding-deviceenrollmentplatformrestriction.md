---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571200"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="bc248-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bc248-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="bc248-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc248-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc248-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="bc248-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="bc248-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc248-106">Properties</span></span>
|<span data-ttu-id="bc248-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc248-107">Property</span></span>|<span data-ttu-id="bc248-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bc248-108">Type</span></span>|<span data-ttu-id="bc248-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bc248-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc248-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="bc248-110">platformBlocked</span></span>|<span data-ttu-id="bc248-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc248-111">Boolean</span></span>|<span data-ttu-id="bc248-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="bc248-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="bc248-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="bc248-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="bc248-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc248-114">Boolean</span></span>|<span data-ttu-id="bc248-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="bc248-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="bc248-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bc248-116">osMinimumVersion</span></span>|<span data-ttu-id="bc248-117">String</span><span class="sxs-lookup"><span data-stu-id="bc248-117">String</span></span>|<span data-ttu-id="bc248-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="bc248-118">Min OS version supported</span></span>|
|<span data-ttu-id="bc248-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bc248-119">osMaximumVersion</span></span>|<span data-ttu-id="bc248-120">String</span><span class="sxs-lookup"><span data-stu-id="bc248-120">String</span></span>|<span data-ttu-id="bc248-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="bc248-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc248-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc248-122">Relationships</span></span>
<span data-ttu-id="bc248-123">Нет</span><span class="sxs-lookup"><span data-stu-id="bc248-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc248-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc248-124">JSON Representation</span></span>
<span data-ttu-id="bc248-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc248-125">Here is a JSON representation of the resource.</span></span>
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



