---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26f29427dfe863ed1b89eaef5025655dc07430fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636597"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2c7ec-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2c7ec-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2c7ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c7ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c7ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c7ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c7ec-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="2c7ec-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="2c7ec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c7ec-107">Properties</span></span>
|<span data-ttu-id="2c7ec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c7ec-108">Property</span></span>|<span data-ttu-id="2c7ec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2c7ec-109">Type</span></span>|<span data-ttu-id="2c7ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c7ec-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2c7ec-111">platformBlocked</span></span>|<span data-ttu-id="2c7ec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c7ec-112">Boolean</span></span>|<span data-ttu-id="2c7ec-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="2c7ec-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2c7ec-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2c7ec-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2c7ec-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c7ec-115">Boolean</span></span>|<span data-ttu-id="2c7ec-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="2c7ec-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2c7ec-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2c7ec-117">osMinimumVersion</span></span>|<span data-ttu-id="2c7ec-118">Строка</span><span class="sxs-lookup"><span data-stu-id="2c7ec-118">String</span></span>|<span data-ttu-id="2c7ec-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2c7ec-119">Min OS version supported</span></span>|
|<span data-ttu-id="2c7ec-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2c7ec-120">osMaximumVersion</span></span>|<span data-ttu-id="2c7ec-121">String</span><span class="sxs-lookup"><span data-stu-id="2c7ec-121">String</span></span>|<span data-ttu-id="2c7ec-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2c7ec-122">Max OS version supported</span></span>|
|<span data-ttu-id="2c7ec-123">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="2c7ec-123">blockedManufacturers</span></span>|<span data-ttu-id="2c7ec-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2c7ec-124">String collection</span></span>|<span data-ttu-id="2c7ec-125">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="2c7ec-125">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c7ec-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2c7ec-126">Relationships</span></span>
<span data-ttu-id="2c7ec-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2c7ec-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c7ec-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c7ec-128">JSON Representation</span></span>
<span data-ttu-id="2c7ec-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c7ec-129">Here is a JSON representation of the resource.</span></span>
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
  "osMaximumVersion": "String",
  "blockedManufacturers": [
    "String"
  ]
}
```



