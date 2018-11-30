---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
ms.openlocfilehash: 823eecc37dc8ee4536d5cb63213f2bb80ca5138d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080941"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="1db21-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1db21-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="1db21-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1db21-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1db21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1db21-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1db21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1db21-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="1db21-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="1db21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1db21-108">Properties</span></span>
|<span data-ttu-id="1db21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1db21-109">Property</span></span>|<span data-ttu-id="1db21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1db21-110">Type</span></span>|<span data-ttu-id="1db21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1db21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db21-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="1db21-112">platformBlocked</span></span>|<span data-ttu-id="1db21-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1db21-113">Boolean</span></span>|<span data-ttu-id="1db21-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="1db21-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="1db21-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="1db21-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="1db21-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1db21-116">Boolean</span></span>|<span data-ttu-id="1db21-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="1db21-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="1db21-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1db21-118">osMinimumVersion</span></span>|<span data-ttu-id="1db21-119">String</span><span class="sxs-lookup"><span data-stu-id="1db21-119">String</span></span>|<span data-ttu-id="1db21-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="1db21-120">Min OS version supported</span></span>|
|<span data-ttu-id="1db21-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1db21-121">osMaximumVersion</span></span>|<span data-ttu-id="1db21-122">String</span><span class="sxs-lookup"><span data-stu-id="1db21-122">String</span></span>|<span data-ttu-id="1db21-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="1db21-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="1db21-124">Связи</span><span class="sxs-lookup"><span data-stu-id="1db21-124">Relationships</span></span>
<span data-ttu-id="1db21-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1db21-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1db21-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1db21-126">JSON Representation</span></span>
<span data-ttu-id="1db21-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1db21-127">Here is a JSON representation of the resource.</span></span>
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





