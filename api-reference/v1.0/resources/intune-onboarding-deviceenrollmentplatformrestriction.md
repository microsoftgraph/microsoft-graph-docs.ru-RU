---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7879b7f6585908aa760c3169e950cc5257bf49a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929069"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="71f18-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71f18-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="71f18-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71f18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71f18-105">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="71f18-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="71f18-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="71f18-106">Properties</span></span>
|<span data-ttu-id="71f18-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="71f18-107">Property</span></span>|<span data-ttu-id="71f18-108">Тип</span><span class="sxs-lookup"><span data-stu-id="71f18-108">Type</span></span>|<span data-ttu-id="71f18-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71f18-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f18-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="71f18-110">platformBlocked</span></span>|<span data-ttu-id="71f18-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="71f18-111">Boolean</span></span>|<span data-ttu-id="71f18-112">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="71f18-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="71f18-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="71f18-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="71f18-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="71f18-114">Boolean</span></span>|<span data-ttu-id="71f18-115">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="71f18-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="71f18-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="71f18-116">osMinimumVersion</span></span>|<span data-ttu-id="71f18-117">String</span><span class="sxs-lookup"><span data-stu-id="71f18-117">String</span></span>|<span data-ttu-id="71f18-118">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="71f18-118">Min OS version supported</span></span>|
|<span data-ttu-id="71f18-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="71f18-119">osMaximumVersion</span></span>|<span data-ttu-id="71f18-120">String</span><span class="sxs-lookup"><span data-stu-id="71f18-120">String</span></span>|<span data-ttu-id="71f18-121">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="71f18-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="71f18-122">Связи</span><span class="sxs-lookup"><span data-stu-id="71f18-122">Relationships</span></span>
<span data-ttu-id="71f18-123">Нет</span><span class="sxs-lookup"><span data-stu-id="71f18-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71f18-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71f18-124">JSON Representation</span></span>
<span data-ttu-id="71f18-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71f18-125">Here is a JSON representation of the resource.</span></span>
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



