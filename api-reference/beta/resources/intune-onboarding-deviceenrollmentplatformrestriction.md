---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf67d9b39462a11286420a6cd6aa79f2e45fb246
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779627"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="ade8c-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ade8c-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="ade8c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ade8c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ade8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ade8c-106">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="ade8c-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="ade8c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ade8c-107">Properties</span></span>
|<span data-ttu-id="ade8c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ade8c-108">Property</span></span>|<span data-ttu-id="ade8c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ade8c-109">Type</span></span>|<span data-ttu-id="ade8c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ade8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ade8c-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="ade8c-111">platformBlocked</span></span>|<span data-ttu-id="ade8c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="ade8c-112">Boolean</span></span>|<span data-ttu-id="ade8c-113">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="ade8c-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="ade8c-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="ade8c-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="ade8c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ade8c-115">Boolean</span></span>|<span data-ttu-id="ade8c-116">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="ade8c-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="ade8c-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ade8c-117">osMinimumVersion</span></span>|<span data-ttu-id="ade8c-118">String</span><span class="sxs-lookup"><span data-stu-id="ade8c-118">String</span></span>|<span data-ttu-id="ade8c-119">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="ade8c-119">Min OS version supported</span></span>|
|<span data-ttu-id="ade8c-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ade8c-120">osMaximumVersion</span></span>|<span data-ttu-id="ade8c-121">String</span><span class="sxs-lookup"><span data-stu-id="ade8c-121">String</span></span>|<span data-ttu-id="ade8c-122">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="ade8c-122">Max OS version supported</span></span>|
|<span data-ttu-id="ade8c-123">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="ade8c-123">blockedManufacturers</span></span>|<span data-ttu-id="ade8c-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ade8c-124">String collection</span></span>|<span data-ttu-id="ade8c-125">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="ade8c-125">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ade8c-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ade8c-126">Relationships</span></span>
<span data-ttu-id="ade8c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ade8c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ade8c-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ade8c-128">JSON Representation</span></span>
<span data-ttu-id="ade8c-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ade8c-129">Here is a JSON representation of the resource.</span></span>
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



