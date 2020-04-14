---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f11a2b0bb3260d834900955886ad477030fd3351
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473538"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="86fe5-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="86fe5-103">reportRoot resource type</span></span>

<span data-ttu-id="86fe5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86fe5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86fe5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86fe5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86fe5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86fe5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86fe5-107">Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="86fe5-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="86fe5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="86fe5-108">Methods</span></span>
|<span data-ttu-id="86fe5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="86fe5-109">Method</span></span>|<span data-ttu-id="86fe5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="86fe5-110">Return Type</span></span>|<span data-ttu-id="86fe5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86fe5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86fe5-112">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="86fe5-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="86fe5-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="86fe5-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="86fe5-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="86fe5-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="86fe5-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="86fe5-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="86fe5-116">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="86fe5-116">**Device configuration**</span></span>|
|[<span data-ttu-id="86fe5-117">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="86fe5-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="86fe5-118">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="86fe5-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="86fe5-119">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="86fe5-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="86fe5-120">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="86fe5-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="86fe5-121">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="86fe5-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="86fe5-122">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="86fe5-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="86fe5-123">report</span><span class="sxs-lookup"><span data-stu-id="86fe5-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="86fe5-124">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="86fe5-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="86fe5-125">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="86fe5-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="86fe5-126">report</span><span class="sxs-lookup"><span data-stu-id="86fe5-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="86fe5-127">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="86fe5-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="86fe5-128">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="86fe5-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="86fe5-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="86fe5-129">Not yet documented</span></span>|
|[<span data-ttu-id="86fe5-130">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="86fe5-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="86fe5-131">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="86fe5-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="86fe5-132">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="86fe5-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="86fe5-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="86fe5-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="86fe5-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="86fe5-134">Properties</span></span>
|<span data-ttu-id="86fe5-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="86fe5-135">Property</span></span>|<span data-ttu-id="86fe5-136">Тип</span><span class="sxs-lookup"><span data-stu-id="86fe5-136">Type</span></span>|<span data-ttu-id="86fe5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="86fe5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86fe5-138">id</span><span class="sxs-lookup"><span data-stu-id="86fe5-138">id</span></span>|<span data-ttu-id="86fe5-139">String</span><span class="sxs-lookup"><span data-stu-id="86fe5-139">String</span></span>|<span data-ttu-id="86fe5-140">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="86fe5-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86fe5-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="86fe5-141">Relationships</span></span>
<span data-ttu-id="86fe5-142">Нет</span><span class="sxs-lookup"><span data-stu-id="86fe5-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86fe5-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86fe5-143">JSON Representation</span></span>
<span data-ttu-id="86fe5-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86fe5-144">Here is a JSON representation of the resource.</span></span>
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



