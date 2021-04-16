---
title: Тип ресурса reportRoot
description: Ресурс, представляюющий экземпляр отчета об устройстве или устранении неполадок, в зависимости от контекста.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30b84ec908eea116442284d6c20e2b56be68ea3c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863648"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="34d01-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="34d01-103">reportRoot resource type</span></span>

<span data-ttu-id="34d01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34d01-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34d01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34d01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34d01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34d01-107">Ресурс, представляюющий экземпляр отчета об устройстве или устранении неполадок, в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="34d01-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="34d01-108">Методы</span><span class="sxs-lookup"><span data-stu-id="34d01-108">Methods</span></span>
|<span data-ttu-id="34d01-109">Метод</span><span class="sxs-lookup"><span data-stu-id="34d01-109">Method</span></span>|<span data-ttu-id="34d01-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34d01-110">Return Type</span></span>|<span data-ttu-id="34d01-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34d01-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34d01-112">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="34d01-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="34d01-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="34d01-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="34d01-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="34d01-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="34d01-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="34d01-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="34d01-116">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="34d01-116">**Device configuration**</span></span>|
|[<span data-ttu-id="34d01-117">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="34d01-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="34d01-118">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="34d01-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="34d01-119">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="34d01-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="34d01-120">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="34d01-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="34d01-121">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="34d01-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="34d01-122">функция managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="34d01-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="34d01-123">report</span><span class="sxs-lookup"><span data-stu-id="34d01-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="34d01-124">Отчет о метаданных для отказа от регистрации</span><span class="sxs-lookup"><span data-stu-id="34d01-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="34d01-125">функция managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="34d01-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="34d01-126">report</span><span class="sxs-lookup"><span data-stu-id="34d01-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="34d01-127">Метаданные для сводного отчета об отказе от регистрации</span><span class="sxs-lookup"><span data-stu-id="34d01-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="34d01-128">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="34d01-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="34d01-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="34d01-129">Not yet documented</span></span>|
|[<span data-ttu-id="34d01-130">функция managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="34d01-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="34d01-131">Метаданные для отчета о тенденциях отказа регистрации</span><span class="sxs-lookup"><span data-stu-id="34d01-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="34d01-132">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="34d01-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="34d01-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="34d01-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="34d01-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="34d01-134">Properties</span></span>
|<span data-ttu-id="34d01-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="34d01-135">Property</span></span>|<span data-ttu-id="34d01-136">Тип</span><span class="sxs-lookup"><span data-stu-id="34d01-136">Type</span></span>|<span data-ttu-id="34d01-137">Описание</span><span class="sxs-lookup"><span data-stu-id="34d01-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d01-138">id</span><span class="sxs-lookup"><span data-stu-id="34d01-138">id</span></span>|<span data-ttu-id="34d01-139">String</span><span class="sxs-lookup"><span data-stu-id="34d01-139">String</span></span>|<span data-ttu-id="34d01-140">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="34d01-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34d01-141">Связи</span><span class="sxs-lookup"><span data-stu-id="34d01-141">Relationships</span></span>
<span data-ttu-id="34d01-142">Нет</span><span class="sxs-lookup"><span data-stu-id="34d01-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34d01-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34d01-143">JSON Representation</span></span>
<span data-ttu-id="34d01-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34d01-144">Here is a JSON representation of the resource.</span></span>
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




