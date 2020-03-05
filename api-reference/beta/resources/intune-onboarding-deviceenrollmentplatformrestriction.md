---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed769c1e6550584688324f4bfdf2db772feae19c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524190"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="0a44b-103">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0a44b-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="0a44b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0a44b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a44b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a44b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a44b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a44b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a44b-107">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="0a44b-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="0a44b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a44b-108">Properties</span></span>
|<span data-ttu-id="0a44b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a44b-109">Property</span></span>|<span data-ttu-id="0a44b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a44b-110">Type</span></span>|<span data-ttu-id="0a44b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a44b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a44b-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="0a44b-112">platformBlocked</span></span>|<span data-ttu-id="0a44b-113">Логический</span><span class="sxs-lookup"><span data-stu-id="0a44b-113">Boolean</span></span>|<span data-ttu-id="0a44b-114">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="0a44b-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="0a44b-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="0a44b-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="0a44b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a44b-116">Boolean</span></span>|<span data-ttu-id="0a44b-117">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="0a44b-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="0a44b-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0a44b-118">osMinimumVersion</span></span>|<span data-ttu-id="0a44b-119">String</span><span class="sxs-lookup"><span data-stu-id="0a44b-119">String</span></span>|<span data-ttu-id="0a44b-120">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0a44b-120">Min OS version supported</span></span>|
|<span data-ttu-id="0a44b-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0a44b-121">osMaximumVersion</span></span>|<span data-ttu-id="0a44b-122">String</span><span class="sxs-lookup"><span data-stu-id="0a44b-122">String</span></span>|<span data-ttu-id="0a44b-123">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="0a44b-123">Max OS version supported</span></span>|
|<span data-ttu-id="0a44b-124">блоккедмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="0a44b-124">blockedManufacturers</span></span>|<span data-ttu-id="0a44b-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a44b-125">String collection</span></span>|<span data-ttu-id="0a44b-126">Коллекция заблокированных производителей.</span><span class="sxs-lookup"><span data-stu-id="0a44b-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a44b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="0a44b-127">Relationships</span></span>
<span data-ttu-id="0a44b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0a44b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a44b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a44b-129">JSON Representation</span></span>
<span data-ttu-id="0a44b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a44b-130">Here is a JSON representation of the resource.</span></span>
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



