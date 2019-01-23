---
title: Тип ресурса reportRoot
description: Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421335"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="784e9-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="784e9-103">reportRoot resource type</span></span>

> <span data-ttu-id="784e9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="784e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="784e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="784e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="784e9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="784e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="784e9-107">Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="784e9-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="784e9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="784e9-108">Methods</span></span>
|<span data-ttu-id="784e9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="784e9-109">Method</span></span>|<span data-ttu-id="784e9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="784e9-110">Return Type</span></span>|<span data-ttu-id="784e9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="784e9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="784e9-112">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="784e9-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="784e9-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="784e9-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="784e9-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="784e9-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="784e9-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="784e9-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="784e9-116">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="784e9-116">**Device configuration**</span></span>|
|[<span data-ttu-id="784e9-117">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="784e9-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="784e9-118">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="784e9-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="784e9-119">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="784e9-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="784e9-120">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="784e9-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="784e9-121">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="784e9-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="784e9-122">функция managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="784e9-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="784e9-123">report</span><span class="sxs-lookup"><span data-stu-id="784e9-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="784e9-124">Метаданные для отчета о регистрации abandonment</span><span class="sxs-lookup"><span data-stu-id="784e9-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="784e9-125">функция managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="784e9-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="784e9-126">report</span><span class="sxs-lookup"><span data-stu-id="784e9-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="784e9-127">Метаданные для регистрации abandonment сводного отчета</span><span class="sxs-lookup"><span data-stu-id="784e9-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="784e9-128">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="784e9-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="784e9-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="784e9-129">Not yet documented</span></span>|
|[<span data-ttu-id="784e9-130">функция managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="784e9-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="784e9-131">Метаданные для отчета тенденций сбой подачи заявок</span><span class="sxs-lookup"><span data-stu-id="784e9-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="784e9-132">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="784e9-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="784e9-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="784e9-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="784e9-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="784e9-134">Properties</span></span>
|<span data-ttu-id="784e9-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="784e9-135">Property</span></span>|<span data-ttu-id="784e9-136">Тип</span><span class="sxs-lookup"><span data-stu-id="784e9-136">Type</span></span>|<span data-ttu-id="784e9-137">Описание</span><span class="sxs-lookup"><span data-stu-id="784e9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="784e9-138">id</span><span class="sxs-lookup"><span data-stu-id="784e9-138">id</span></span>|<span data-ttu-id="784e9-139">String</span><span class="sxs-lookup"><span data-stu-id="784e9-139">String</span></span>|<span data-ttu-id="784e9-140">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="784e9-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="784e9-141">Связи</span><span class="sxs-lookup"><span data-stu-id="784e9-141">Relationships</span></span>
<span data-ttu-id="784e9-142">Нет</span><span class="sxs-lookup"><span data-stu-id="784e9-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="784e9-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="784e9-143">JSON Representation</span></span>
<span data-ttu-id="784e9-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="784e9-144">Here is a JSON representation of the resource.</span></span>
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



