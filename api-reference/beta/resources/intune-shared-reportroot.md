---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c975abfa3cb580d107967c7adaf66627bad2ad2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938732"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="8b252-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="8b252-103">reportRoot resource type</span></span>

> <span data-ttu-id="8b252-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b252-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b252-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b252-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b252-106">Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="8b252-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="8b252-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8b252-107">Methods</span></span>
|<span data-ttu-id="8b252-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8b252-108">Method</span></span>|<span data-ttu-id="8b252-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8b252-109">Return Type</span></span>|<span data-ttu-id="8b252-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b252-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b252-111">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="8b252-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="8b252-112">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="8b252-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="8b252-113">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="8b252-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="8b252-114">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="8b252-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="8b252-115">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="8b252-115">**Device configuration**</span></span>|
|[<span data-ttu-id="8b252-116">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="8b252-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="8b252-117">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="8b252-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="8b252-118">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="8b252-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="8b252-119">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="8b252-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="8b252-120">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="8b252-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="8b252-121">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="8b252-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="8b252-122">report</span><span class="sxs-lookup"><span data-stu-id="8b252-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="8b252-123">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="8b252-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="8b252-124">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="8b252-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="8b252-125">report</span><span class="sxs-lookup"><span data-stu-id="8b252-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="8b252-126">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="8b252-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="8b252-127">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="8b252-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="8b252-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b252-128">Not yet documented</span></span>|
|[<span data-ttu-id="8b252-129">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="8b252-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="8b252-130">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="8b252-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="8b252-131">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="8b252-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="8b252-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b252-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8b252-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b252-133">Properties</span></span>
|<span data-ttu-id="8b252-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b252-134">Property</span></span>|<span data-ttu-id="8b252-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8b252-135">Type</span></span>|<span data-ttu-id="8b252-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8b252-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b252-137">id</span><span class="sxs-lookup"><span data-stu-id="8b252-137">id</span></span>|<span data-ttu-id="8b252-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8b252-138">String</span></span>|<span data-ttu-id="8b252-139">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="8b252-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b252-140">Связи</span><span class="sxs-lookup"><span data-stu-id="8b252-140">Relationships</span></span>
<span data-ttu-id="8b252-141">Нет</span><span class="sxs-lookup"><span data-stu-id="8b252-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b252-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b252-142">JSON Representation</span></span>
<span data-ttu-id="8b252-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b252-143">Here is a JSON representation of the resource.</span></span>
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



