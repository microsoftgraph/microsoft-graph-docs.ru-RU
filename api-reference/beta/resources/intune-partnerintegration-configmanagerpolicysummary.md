---
title: Тип ресурса Конфигманажерполицисуммари
description: Сводка по политике Конфигманажер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63e85448b70abc76f4df0021c4f5516e778ebe0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302011"
---
# <a name="configmanagerpolicysummary-resource-type"></a><span data-ttu-id="fcc15-103">Тип ресурса Конфигманажерполицисуммари</span><span class="sxs-lookup"><span data-stu-id="fcc15-103">configManagerPolicySummary resource type</span></span>

<span data-ttu-id="fcc15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcc15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcc15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcc15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcc15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcc15-107">Сводка по политике Конфигманажер.</span><span class="sxs-lookup"><span data-stu-id="fcc15-107">A ConfigManager policy summary.</span></span>

## <a name="properties"></a><span data-ttu-id="fcc15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcc15-108">Properties</span></span>
|<span data-ttu-id="fcc15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc15-109">Property</span></span>|<span data-ttu-id="fcc15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc15-110">Type</span></span>|<span data-ttu-id="fcc15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc15-112">таржетеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="fcc15-112">targetedDeviceCount</span></span>|<span data-ttu-id="fcc15-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-113">Int32</span></span>|<span data-ttu-id="fcc15-114">Количество устройств, для которых предназначена политика.</span><span class="sxs-lookup"><span data-stu-id="fcc15-114">The number of devices targeted by the policy.</span></span>|
|<span data-ttu-id="fcc15-115">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcc15-115">compliantDeviceCount</span></span>|<span data-ttu-id="fcc15-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-116">Int32</span></span>|<span data-ttu-id="fcc15-117">Количество устройств, которые оцениваются в соответствии с политикой.</span><span class="sxs-lookup"><span data-stu-id="fcc15-117">The number of devices evaluated to be compliant by the policy.</span></span>|
|<span data-ttu-id="fcc15-118">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcc15-118">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fcc15-119">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-119">Int32</span></span>|<span data-ttu-id="fcc15-120">Количество устройств, которые оцениваются не в соответствии с политикой.</span><span class="sxs-lookup"><span data-stu-id="fcc15-120">The number of devices evaluated to be noncompliant by the policy.</span></span>|
|<span data-ttu-id="fcc15-121">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcc15-121">failedDeviceCount</span></span>|<span data-ttu-id="fcc15-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-122">Int32</span></span>|<span data-ttu-id="fcc15-123">Количество устройств, которые не удалось оценить с помощью политики.</span><span class="sxs-lookup"><span data-stu-id="fcc15-123">The number of devices that failed to be evaluated by the policy.</span></span>|
|<span data-ttu-id="fcc15-124">пендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="fcc15-124">pendingDeviceCount</span></span>|<span data-ttu-id="fcc15-125">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-125">Int32</span></span>|<span data-ttu-id="fcc15-126">Количество устройств, которые подтвердили политику, но ожидают оценки.</span><span class="sxs-lookup"><span data-stu-id="fcc15-126">The number of devices that have acknowledged the policy but are pending evaluation.</span></span>|
|<span data-ttu-id="fcc15-127">енфорцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="fcc15-127">enforcedDeviceCount</span></span>|<span data-ttu-id="fcc15-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc15-128">Int32</span></span>|<span data-ttu-id="fcc15-129">Количество устройств, исправленных политикой.</span><span class="sxs-lookup"><span data-stu-id="fcc15-129">The number of devices that have have been remediated by the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcc15-130">Связи</span><span class="sxs-lookup"><span data-stu-id="fcc15-130">Relationships</span></span>
<span data-ttu-id="fcc15-131">Нет</span><span class="sxs-lookup"><span data-stu-id="fcc15-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcc15-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcc15-132">JSON Representation</span></span>
<span data-ttu-id="fcc15-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc15-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configManagerPolicySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerPolicySummary",
  "targetedDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "enforcedDeviceCount": 1024
}
```




