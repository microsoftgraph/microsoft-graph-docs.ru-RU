---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
ms.openlocfilehash: b6d4ea3acf4995548fce7f2c86b3c95c444b59b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028429"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8fe0e-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe0e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="8fe0e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8fe0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fe0e-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="8fe0e-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="8fe0e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fe0e-106">Properties</span></span>
|<span data-ttu-id="8fe0e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fe0e-107">Property</span></span>|<span data-ttu-id="8fe0e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8fe0e-108">Type</span></span>|<span data-ttu-id="8fe0e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8fe0e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe0e-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe0e-110">platformBlocked</span></span>|<span data-ttu-id="8fe0e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe0e-111">Boolean</span></span>|<span data-ttu-id="8fe0e-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="8fe0e-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8fe0e-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8fe0e-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8fe0e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe0e-114">Boolean</span></span>|<span data-ttu-id="8fe0e-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="8fe0e-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8fe0e-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8fe0e-116">osMinimumVersion</span></span>|<span data-ttu-id="8fe0e-117">String</span><span class="sxs-lookup"><span data-stu-id="8fe0e-117">String</span></span>|<span data-ttu-id="8fe0e-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="8fe0e-118">Min OS version supported</span></span>|
|<span data-ttu-id="8fe0e-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8fe0e-119">osMaximumVersion</span></span>|<span data-ttu-id="8fe0e-120">String</span><span class="sxs-lookup"><span data-stu-id="8fe0e-120">String</span></span>|<span data-ttu-id="8fe0e-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="8fe0e-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fe0e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8fe0e-122">Relationships</span></span>
<span data-ttu-id="8fe0e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8fe0e-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fe0e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fe0e-124">JSON Representation</span></span>
<span data-ttu-id="8fe0e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fe0e-125">Here is a JSON representation of the resource.</span></span>
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



