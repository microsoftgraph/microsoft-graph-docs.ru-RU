---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5189b286de61375715944c5ac979d847392a18c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917764"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="0db8e-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0db8e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="0db8e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0db8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0db8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0db8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0db8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0db8e-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="0db8e-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="0db8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0db8e-108">Properties</span></span>
|<span data-ttu-id="0db8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db8e-109">Property</span></span>|<span data-ttu-id="0db8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0db8e-110">Type</span></span>|<span data-ttu-id="0db8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0db8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db8e-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="0db8e-112">platformBlocked</span></span>|<span data-ttu-id="0db8e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0db8e-113">Boolean</span></span>|<span data-ttu-id="0db8e-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="0db8e-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="0db8e-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="0db8e-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="0db8e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0db8e-116">Boolean</span></span>|<span data-ttu-id="0db8e-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="0db8e-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="0db8e-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0db8e-118">osMinimumVersion</span></span>|<span data-ttu-id="0db8e-119">String</span><span class="sxs-lookup"><span data-stu-id="0db8e-119">String</span></span>|<span data-ttu-id="0db8e-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0db8e-120">Min OS version supported</span></span>|
|<span data-ttu-id="0db8e-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0db8e-121">osMaximumVersion</span></span>|<span data-ttu-id="0db8e-122">String</span><span class="sxs-lookup"><span data-stu-id="0db8e-122">String</span></span>|<span data-ttu-id="0db8e-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0db8e-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db8e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0db8e-124">Relationships</span></span>
<span data-ttu-id="0db8e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0db8e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0db8e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0db8e-126">JSON Representation</span></span>
<span data-ttu-id="0db8e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0db8e-127">Here is a JSON representation of the resource.</span></span>
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





