---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 739cdc4bd9b10f9d472cebd77c88ae796593a1f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523578"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="937ce-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="937ce-103">reportRoot resource type</span></span>

<span data-ttu-id="937ce-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="937ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="937ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="937ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="937ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="937ce-107">Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="937ce-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="937ce-108">Методы</span><span class="sxs-lookup"><span data-stu-id="937ce-108">Methods</span></span>
|<span data-ttu-id="937ce-109">Метод</span><span class="sxs-lookup"><span data-stu-id="937ce-109">Method</span></span>|<span data-ttu-id="937ce-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="937ce-110">Return Type</span></span>|<span data-ttu-id="937ce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="937ce-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="937ce-112">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="937ce-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="937ce-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="937ce-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="937ce-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="937ce-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="937ce-116">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="937ce-116">**Device configuration**</span></span>|
|[<span data-ttu-id="937ce-117">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="937ce-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="937ce-118">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="937ce-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="937ce-119">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="937ce-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="937ce-120">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="937ce-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="937ce-121">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="937ce-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="937ce-122">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="937ce-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="937ce-123">report</span><span class="sxs-lookup"><span data-stu-id="937ce-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="937ce-124">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="937ce-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="937ce-125">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="937ce-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="937ce-126">report</span><span class="sxs-lookup"><span data-stu-id="937ce-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="937ce-127">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="937ce-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="937ce-128">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="937ce-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="937ce-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="937ce-129">Not yet documented</span></span>|
|[<span data-ttu-id="937ce-130">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="937ce-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="937ce-131">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="937ce-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="937ce-132">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="937ce-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="937ce-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="937ce-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="937ce-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="937ce-134">Properties</span></span>
|<span data-ttu-id="937ce-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="937ce-135">Property</span></span>|<span data-ttu-id="937ce-136">Тип</span><span class="sxs-lookup"><span data-stu-id="937ce-136">Type</span></span>|<span data-ttu-id="937ce-137">Описание</span><span class="sxs-lookup"><span data-stu-id="937ce-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="937ce-138">id</span><span class="sxs-lookup"><span data-stu-id="937ce-138">id</span></span>|<span data-ttu-id="937ce-139">String</span><span class="sxs-lookup"><span data-stu-id="937ce-139">String</span></span>|<span data-ttu-id="937ce-140">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="937ce-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="937ce-141">Связи</span><span class="sxs-lookup"><span data-stu-id="937ce-141">Relationships</span></span>
<span data-ttu-id="937ce-142">Нет</span><span class="sxs-lookup"><span data-stu-id="937ce-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="937ce-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="937ce-143">JSON Representation</span></span>
<span data-ttu-id="937ce-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="937ce-144">Here is a JSON representation of the resource.</span></span>
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



