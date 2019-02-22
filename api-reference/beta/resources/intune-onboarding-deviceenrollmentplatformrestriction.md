---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eecbc405fd56d21f7be1c7b9bccd5254db89c8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140602"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="f0132-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f0132-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="f0132-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0132-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0132-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="f0132-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="f0132-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0132-107">Properties</span></span>
|<span data-ttu-id="f0132-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0132-108">Property</span></span>|<span data-ttu-id="f0132-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0132-109">Type</span></span>|<span data-ttu-id="f0132-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0132-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0132-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="f0132-111">platformBlocked</span></span>|<span data-ttu-id="f0132-112">Логический</span><span class="sxs-lookup"><span data-stu-id="f0132-112">Boolean</span></span>|<span data-ttu-id="f0132-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="f0132-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="f0132-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="f0132-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="f0132-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0132-115">Boolean</span></span>|<span data-ttu-id="f0132-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="f0132-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="f0132-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f0132-117">osMinimumVersion</span></span>|<span data-ttu-id="f0132-118">String</span><span class="sxs-lookup"><span data-stu-id="f0132-118">String</span></span>|<span data-ttu-id="f0132-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="f0132-119">Min OS version supported</span></span>|
|<span data-ttu-id="f0132-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f0132-120">osMaximumVersion</span></span>|<span data-ttu-id="f0132-121">String</span><span class="sxs-lookup"><span data-stu-id="f0132-121">String</span></span>|<span data-ttu-id="f0132-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="f0132-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0132-123">Связи</span><span class="sxs-lookup"><span data-stu-id="f0132-123">Relationships</span></span>
<span data-ttu-id="f0132-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f0132-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0132-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0132-125">JSON Representation</span></span>
<span data-ttu-id="f0132-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0132-126">Here is a JSON representation of the resource.</span></span>
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




