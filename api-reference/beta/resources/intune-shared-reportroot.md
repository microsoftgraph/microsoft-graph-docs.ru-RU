---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572943"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="87746-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="87746-103">reportRoot resource type</span></span>

> <span data-ttu-id="87746-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87746-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87746-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87746-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87746-106">Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="87746-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="87746-107">Методы</span><span class="sxs-lookup"><span data-stu-id="87746-107">Methods</span></span>
|<span data-ttu-id="87746-108">Метод</span><span class="sxs-lookup"><span data-stu-id="87746-108">Method</span></span>|<span data-ttu-id="87746-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87746-109">Return Type</span></span>|<span data-ttu-id="87746-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87746-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87746-111">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="87746-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="87746-112">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="87746-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="87746-113">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="87746-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="87746-114">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="87746-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="87746-115">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="87746-115">**Device configuration**</span></span>|
|[<span data-ttu-id="87746-116">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="87746-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="87746-117">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="87746-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="87746-118">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="87746-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="87746-119">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="87746-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="87746-120">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="87746-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="87746-121">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="87746-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="87746-122">report</span><span class="sxs-lookup"><span data-stu-id="87746-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="87746-123">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="87746-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="87746-124">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="87746-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="87746-125">report</span><span class="sxs-lookup"><span data-stu-id="87746-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="87746-126">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="87746-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="87746-127">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="87746-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="87746-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="87746-128">Not yet documented</span></span>|
|[<span data-ttu-id="87746-129">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="87746-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="87746-130">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="87746-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="87746-131">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="87746-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="87746-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="87746-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="87746-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="87746-133">Properties</span></span>
|<span data-ttu-id="87746-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="87746-134">Property</span></span>|<span data-ttu-id="87746-135">Тип</span><span class="sxs-lookup"><span data-stu-id="87746-135">Type</span></span>|<span data-ttu-id="87746-136">Описание</span><span class="sxs-lookup"><span data-stu-id="87746-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87746-137">id</span><span class="sxs-lookup"><span data-stu-id="87746-137">id</span></span>|<span data-ttu-id="87746-138">String</span><span class="sxs-lookup"><span data-stu-id="87746-138">String</span></span>|<span data-ttu-id="87746-139">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="87746-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87746-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="87746-140">Relationships</span></span>
<span data-ttu-id="87746-141">Нет</span><span class="sxs-lookup"><span data-stu-id="87746-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87746-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87746-142">JSON Representation</span></span>
<span data-ttu-id="87746-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87746-143">Here is a JSON representation of the resource.</span></span>
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



