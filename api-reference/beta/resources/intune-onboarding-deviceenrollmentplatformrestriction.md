---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
ms.openlocfilehash: 22401c83b3e68d66a2bd7a39359602e2aca0a932
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304125"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="06d03-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06d03-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="06d03-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06d03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06d03-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06d03-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06d03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06d03-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="06d03-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="06d03-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="06d03-108">Properties</span></span>
|<span data-ttu-id="06d03-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="06d03-109">Property</span></span>|<span data-ttu-id="06d03-110">Тип</span><span class="sxs-lookup"><span data-stu-id="06d03-110">Type</span></span>|<span data-ttu-id="06d03-111">Описание</span><span class="sxs-lookup"><span data-stu-id="06d03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d03-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="06d03-112">platformBlocked</span></span>|<span data-ttu-id="06d03-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d03-113">Boolean</span></span>|<span data-ttu-id="06d03-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="06d03-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="06d03-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="06d03-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="06d03-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d03-116">Boolean</span></span>|<span data-ttu-id="06d03-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="06d03-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="06d03-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06d03-118">osMinimumVersion</span></span>|<span data-ttu-id="06d03-119">String</span><span class="sxs-lookup"><span data-stu-id="06d03-119">String</span></span>|<span data-ttu-id="06d03-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="06d03-120">Min OS version supported</span></span>|
|<span data-ttu-id="06d03-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06d03-121">osMaximumVersion</span></span>|<span data-ttu-id="06d03-122">String</span><span class="sxs-lookup"><span data-stu-id="06d03-122">String</span></span>|<span data-ttu-id="06d03-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="06d03-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="06d03-124">Связи</span><span class="sxs-lookup"><span data-stu-id="06d03-124">Relationships</span></span>
<span data-ttu-id="06d03-125">Нет</span><span class="sxs-lookup"><span data-stu-id="06d03-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06d03-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06d03-126">JSON Representation</span></span>
<span data-ttu-id="06d03-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06d03-127">Here is a JSON representation of the resource.</span></span>
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





