---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0e7fc15987c7d9e13ecc1f2cd44aa3869556b2f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767969"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="fe02c-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="fe02c-103">reportRoot resource type</span></span>

> <span data-ttu-id="fe02c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe02c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe02c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe02c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe02c-106">Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="fe02c-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="fe02c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fe02c-107">Methods</span></span>
|<span data-ttu-id="fe02c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fe02c-108">Method</span></span>|<span data-ttu-id="fe02c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe02c-109">Return Type</span></span>|<span data-ttu-id="fe02c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe02c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe02c-111">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="fe02c-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="fe02c-112">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fe02c-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="fe02c-113">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="fe02c-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="fe02c-114">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fe02c-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="fe02c-115">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="fe02c-115">**Device configuration**</span></span>|
|[<span data-ttu-id="fe02c-116">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="fe02c-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="fe02c-117">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="fe02c-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="fe02c-118">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="fe02c-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="fe02c-119">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="fe02c-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="fe02c-120">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="fe02c-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="fe02c-121">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="fe02c-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="fe02c-122">report</span><span class="sxs-lookup"><span data-stu-id="fe02c-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="fe02c-123">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="fe02c-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="fe02c-124">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="fe02c-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="fe02c-125">report</span><span class="sxs-lookup"><span data-stu-id="fe02c-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="fe02c-126">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="fe02c-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="fe02c-127">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="fe02c-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="fe02c-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fe02c-128">Not yet documented</span></span>|
|[<span data-ttu-id="fe02c-129">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="fe02c-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="fe02c-130">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="fe02c-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="fe02c-131">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="fe02c-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="fe02c-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fe02c-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fe02c-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe02c-133">Properties</span></span>
|<span data-ttu-id="fe02c-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe02c-134">Property</span></span>|<span data-ttu-id="fe02c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="fe02c-135">Type</span></span>|<span data-ttu-id="fe02c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fe02c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe02c-137">id</span><span class="sxs-lookup"><span data-stu-id="fe02c-137">id</span></span>|<span data-ttu-id="fe02c-138">String</span><span class="sxs-lookup"><span data-stu-id="fe02c-138">String</span></span>|<span data-ttu-id="fe02c-139">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="fe02c-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe02c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="fe02c-140">Relationships</span></span>
<span data-ttu-id="fe02c-141">Нет</span><span class="sxs-lookup"><span data-stu-id="fe02c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe02c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe02c-142">JSON Representation</span></span>
<span data-ttu-id="fe02c-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe02c-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



