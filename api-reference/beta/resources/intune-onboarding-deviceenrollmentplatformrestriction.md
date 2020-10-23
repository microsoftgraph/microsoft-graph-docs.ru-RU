---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6fdb900b9f9ce5c89828e6e945623a766de2041
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697240"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="db134-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="db134-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="db134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db134-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db134-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db134-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db134-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db134-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db134-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="db134-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="db134-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="db134-108">Properties</span></span>
|<span data-ttu-id="db134-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="db134-109">Property</span></span>|<span data-ttu-id="db134-110">Тип</span><span class="sxs-lookup"><span data-stu-id="db134-110">Type</span></span>|<span data-ttu-id="db134-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db134-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db134-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="db134-112">platformBlocked</span></span>|<span data-ttu-id="db134-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="db134-113">Boolean</span></span>|<span data-ttu-id="db134-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="db134-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="db134-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="db134-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="db134-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="db134-116">Boolean</span></span>|<span data-ttu-id="db134-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="db134-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="db134-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="db134-118">osMinimumVersion</span></span>|<span data-ttu-id="db134-119">String</span><span class="sxs-lookup"><span data-stu-id="db134-119">String</span></span>|<span data-ttu-id="db134-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="db134-120">Min OS version supported</span></span>|
|<span data-ttu-id="db134-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="db134-121">osMaximumVersion</span></span>|<span data-ttu-id="db134-122">String</span><span class="sxs-lookup"><span data-stu-id="db134-122">String</span></span>|<span data-ttu-id="db134-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="db134-123">Max OS version supported</span></span>|
|<span data-ttu-id="db134-124">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="db134-124">blockedManufacturers</span></span>|<span data-ttu-id="db134-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db134-125">String collection</span></span>|<span data-ttu-id="db134-126">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="db134-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db134-127">Связи</span><span class="sxs-lookup"><span data-stu-id="db134-127">Relationships</span></span>
<span data-ttu-id="db134-128">Нет</span><span class="sxs-lookup"><span data-stu-id="db134-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db134-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db134-129">JSON Representation</span></span>
<span data-ttu-id="db134-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db134-130">Here is a JSON representation of the resource.</span></span>
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





