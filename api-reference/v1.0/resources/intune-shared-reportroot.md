---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9724f3f67ce31bcb781adad4107f3f0e6f59e620
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962060"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="455a8-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="455a8-103">reportRoot resource type</span></span>

> <span data-ttu-id="455a8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="455a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="455a8-105">Ресурс, представляющий экземпляр отчетов журнала.</span><span class="sxs-lookup"><span data-stu-id="455a8-105">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="455a8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="455a8-106">Methods</span></span>
|<span data-ttu-id="455a8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="455a8-107">Method</span></span>|<span data-ttu-id="455a8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="455a8-108">Return Type</span></span>|<span data-ttu-id="455a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="455a8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="455a8-110">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="455a8-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="455a8-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="455a8-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="455a8-112">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="455a8-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="455a8-113">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="455a8-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="455a8-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="455a8-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="455a8-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="455a8-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="455a8-116">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="455a8-116">**Device configuration**</span></span>|
|[<span data-ttu-id="455a8-117">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="455a8-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="455a8-118">report</span><span class="sxs-lookup"><span data-stu-id="455a8-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="455a8-119">Метаданные для отчета о действиях устройств с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="455a8-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="455a8-120">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="455a8-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="455a8-121">report</span><span class="sxs-lookup"><span data-stu-id="455a8-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="455a8-122">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="455a8-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="455a8-123">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="455a8-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="455a8-124">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="455a8-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="455a8-125">report</span><span class="sxs-lookup"><span data-stu-id="455a8-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="455a8-126">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="455a8-126">Not yet documented.</span></span>|
|[<span data-ttu-id="455a8-127">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="455a8-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="455a8-128">report</span><span class="sxs-lookup"><span data-stu-id="455a8-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="455a8-129">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="455a8-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="455a8-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="455a8-130">Properties</span></span>
|<span data-ttu-id="455a8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="455a8-131">Property</span></span>|<span data-ttu-id="455a8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="455a8-132">Type</span></span>|<span data-ttu-id="455a8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="455a8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455a8-134">id</span><span class="sxs-lookup"><span data-stu-id="455a8-134">id</span></span>|<span data-ttu-id="455a8-135">String</span><span class="sxs-lookup"><span data-stu-id="455a8-135">String</span></span>|<span data-ttu-id="455a8-136">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="455a8-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="455a8-137">Связи</span><span class="sxs-lookup"><span data-stu-id="455a8-137">Relationships</span></span>
<span data-ttu-id="455a8-138">Нет</span><span class="sxs-lookup"><span data-stu-id="455a8-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="455a8-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="455a8-139">JSON Representation</span></span>
<span data-ttu-id="455a8-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="455a8-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a><span data-ttu-id="455a8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="455a8-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
