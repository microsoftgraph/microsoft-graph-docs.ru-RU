---
title: Тип ресурса reportRoot
description: Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: efb8950b9956901161c822df8b467b0182a4cc75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959589"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="b2e15-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="b2e15-103">reportRoot resource type</span></span>

> <span data-ttu-id="b2e15-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2e15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2e15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2e15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2e15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2e15-107">Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="b2e15-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="b2e15-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b2e15-108">Methods</span></span>
|<span data-ttu-id="b2e15-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b2e15-109">Method</span></span>|<span data-ttu-id="b2e15-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2e15-110">Return Type</span></span>|<span data-ttu-id="b2e15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e15-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b2e15-112">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="b2e15-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="b2e15-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b2e15-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="b2e15-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="b2e15-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="b2e15-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b2e15-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="b2e15-116">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="b2e15-116">**Device configuration**</span></span>|
|[<span data-ttu-id="b2e15-117">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="b2e15-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="b2e15-118">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="b2e15-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="b2e15-119">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="b2e15-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="b2e15-120">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="b2e15-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="b2e15-121">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b2e15-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="b2e15-122">функция managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="b2e15-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="b2e15-123">report</span><span class="sxs-lookup"><span data-stu-id="b2e15-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="b2e15-124">Метаданные для отчета о регистрации abandonment</span><span class="sxs-lookup"><span data-stu-id="b2e15-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="b2e15-125">функция managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="b2e15-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="b2e15-126">report</span><span class="sxs-lookup"><span data-stu-id="b2e15-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="b2e15-127">Метаданные для регистрации abandonment сводного отчета</span><span class="sxs-lookup"><span data-stu-id="b2e15-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="b2e15-128">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="b2e15-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="b2e15-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2e15-129">Not yet documented</span></span>|
|[<span data-ttu-id="b2e15-130">функция managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="b2e15-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="b2e15-131">Метаданные для отчета тенденций сбой подачи заявок</span><span class="sxs-lookup"><span data-stu-id="b2e15-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="b2e15-132">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="b2e15-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="b2e15-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2e15-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b2e15-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e15-134">Properties</span></span>
|<span data-ttu-id="b2e15-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e15-135">Property</span></span>|<span data-ttu-id="b2e15-136">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e15-136">Type</span></span>|<span data-ttu-id="b2e15-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e15-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e15-138">id</span><span class="sxs-lookup"><span data-stu-id="b2e15-138">id</span></span>|<span data-ttu-id="b2e15-139">String</span><span class="sxs-lookup"><span data-stu-id="b2e15-139">String</span></span>|<span data-ttu-id="b2e15-140">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="b2e15-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2e15-141">Связи</span><span class="sxs-lookup"><span data-stu-id="b2e15-141">Relationships</span></span>
<span data-ttu-id="b2e15-142">Нет</span><span class="sxs-lookup"><span data-stu-id="b2e15-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e15-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2e15-143">JSON Representation</span></span>
<span data-ttu-id="b2e15-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e15-144">Here is a JSON representation of the resource.</span></span>
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



