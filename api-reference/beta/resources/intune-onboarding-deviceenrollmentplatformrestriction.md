---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 255e9b815657fa354ab4180e8685049ec78ed585
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029752"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="0cbb3-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0cbb3-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="0cbb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cbb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cbb3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cbb3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cbb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cbb3-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="0cbb3-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="0cbb3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cbb3-108">Properties</span></span>
|<span data-ttu-id="0cbb3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cbb3-109">Property</span></span>|<span data-ttu-id="0cbb3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0cbb3-110">Type</span></span>|<span data-ttu-id="0cbb3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0cbb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cbb3-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="0cbb3-112">platformBlocked</span></span>|<span data-ttu-id="0cbb3-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cbb3-113">Boolean</span></span>|<span data-ttu-id="0cbb3-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="0cbb3-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="0cbb3-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="0cbb3-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="0cbb3-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cbb3-116">Boolean</span></span>|<span data-ttu-id="0cbb3-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="0cbb3-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="0cbb3-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0cbb3-118">osMinimumVersion</span></span>|<span data-ttu-id="0cbb3-119">String</span><span class="sxs-lookup"><span data-stu-id="0cbb3-119">String</span></span>|<span data-ttu-id="0cbb3-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0cbb3-120">Min OS version supported</span></span>|
|<span data-ttu-id="0cbb3-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0cbb3-121">osMaximumVersion</span></span>|<span data-ttu-id="0cbb3-122">String</span><span class="sxs-lookup"><span data-stu-id="0cbb3-122">String</span></span>|<span data-ttu-id="0cbb3-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0cbb3-123">Max OS version supported</span></span>|
|<span data-ttu-id="0cbb3-124">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="0cbb3-124">blockedManufacturers</span></span>|<span data-ttu-id="0cbb3-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0cbb3-125">String collection</span></span>|<span data-ttu-id="0cbb3-126">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="0cbb3-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cbb3-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="0cbb3-127">Relationships</span></span>
<span data-ttu-id="0cbb3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0cbb3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cbb3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cbb3-129">JSON Representation</span></span>
<span data-ttu-id="0cbb3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cbb3-130">Here is a JSON representation of the resource.</span></span>
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






