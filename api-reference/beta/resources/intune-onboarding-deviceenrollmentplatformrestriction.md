---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05105eec5b3b870ee608d0b47861d1eaddae8965
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301279"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2ea58-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2ea58-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="2ea58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ea58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ea58-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ea58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ea58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ea58-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="2ea58-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="2ea58-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ea58-108">Properties</span></span>
|<span data-ttu-id="2ea58-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ea58-109">Property</span></span>|<span data-ttu-id="2ea58-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2ea58-110">Type</span></span>|<span data-ttu-id="2ea58-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea58-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2ea58-112">platformBlocked</span></span>|<span data-ttu-id="2ea58-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ea58-113">Boolean</span></span>|<span data-ttu-id="2ea58-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="2ea58-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2ea58-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2ea58-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2ea58-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ea58-116">Boolean</span></span>|<span data-ttu-id="2ea58-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="2ea58-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2ea58-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2ea58-118">osMinimumVersion</span></span>|<span data-ttu-id="2ea58-119">String</span><span class="sxs-lookup"><span data-stu-id="2ea58-119">String</span></span>|<span data-ttu-id="2ea58-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2ea58-120">Min OS version supported</span></span>|
|<span data-ttu-id="2ea58-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2ea58-121">osMaximumVersion</span></span>|<span data-ttu-id="2ea58-122">String</span><span class="sxs-lookup"><span data-stu-id="2ea58-122">String</span></span>|<span data-ttu-id="2ea58-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="2ea58-123">Max OS version supported</span></span>|
|<span data-ttu-id="2ea58-124">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="2ea58-124">blockedManufacturers</span></span>|<span data-ttu-id="2ea58-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ea58-125">String collection</span></span>|<span data-ttu-id="2ea58-126">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="2ea58-126">Collection of blocked Manufacturers.</span></span>|
|<span data-ttu-id="2ea58-127">блоккедскус</span><span class="sxs-lookup"><span data-stu-id="2ea58-127">blockedSkus</span></span>|<span data-ttu-id="2ea58-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ea58-128">String collection</span></span>|<span data-ttu-id="2ea58-129">Коллекция заблокированных SKU.</span><span class="sxs-lookup"><span data-stu-id="2ea58-129">Collection of blocked Skus.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ea58-130">Связи</span><span class="sxs-lookup"><span data-stu-id="2ea58-130">Relationships</span></span>
<span data-ttu-id="2ea58-131">Нет</span><span class="sxs-lookup"><span data-stu-id="2ea58-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ea58-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ea58-132">JSON Representation</span></span>
<span data-ttu-id="2ea58-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ea58-133">Here is a JSON representation of the resource.</span></span>
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
  ],
  "blockedSkus": [
    "String"
  ]
}
```




