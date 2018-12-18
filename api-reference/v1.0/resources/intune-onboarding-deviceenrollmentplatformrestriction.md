---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
ms.openlocfilehash: cccac8240457ffe2b5c27475e8ac9e8fb83200ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329388"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2551a-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2551a-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2551a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2551a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2551a-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="2551a-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="2551a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2551a-106">Properties</span></span>
|<span data-ttu-id="2551a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2551a-107">Property</span></span>|<span data-ttu-id="2551a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2551a-108">Type</span></span>|<span data-ttu-id="2551a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2551a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2551a-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2551a-110">platformBlocked</span></span>|<span data-ttu-id="2551a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2551a-111">Boolean</span></span>|<span data-ttu-id="2551a-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="2551a-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2551a-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2551a-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2551a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2551a-114">Boolean</span></span>|<span data-ttu-id="2551a-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="2551a-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2551a-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2551a-116">osMinimumVersion</span></span>|<span data-ttu-id="2551a-117">String</span><span class="sxs-lookup"><span data-stu-id="2551a-117">String</span></span>|<span data-ttu-id="2551a-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2551a-118">Min OS version supported</span></span>|
|<span data-ttu-id="2551a-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2551a-119">osMaximumVersion</span></span>|<span data-ttu-id="2551a-120">String</span><span class="sxs-lookup"><span data-stu-id="2551a-120">String</span></span>|<span data-ttu-id="2551a-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2551a-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2551a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="2551a-122">Relationships</span></span>
<span data-ttu-id="2551a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2551a-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2551a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2551a-124">JSON Representation</span></span>
<span data-ttu-id="2551a-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2551a-125">Here is a JSON representation of the resource.</span></span>
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



