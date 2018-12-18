---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: tfitzmac
ms.openlocfilehash: 46b4844487a1cb714dde791e6867c277c1693f66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303971"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="d246b-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="d246b-103">reportRoot resource type</span></span>

> <span data-ttu-id="d246b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d246b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d246b-105">Ресурс, представляющий экземпляр отчетов журнала.</span><span class="sxs-lookup"><span data-stu-id="d246b-105">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="d246b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d246b-106">Methods</span></span>
|<span data-ttu-id="d246b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d246b-107">Method</span></span>|<span data-ttu-id="d246b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d246b-108">Return Type</span></span>|<span data-ttu-id="d246b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d246b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d246b-110">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="d246b-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="d246b-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d246b-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="d246b-112">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d246b-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="d246b-113">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="d246b-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="d246b-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d246b-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="d246b-115">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d246b-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="d246b-116">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d246b-116">**Device configuration**</span></span>|
|[<span data-ttu-id="d246b-117">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="d246b-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="d246b-118">report</span><span class="sxs-lookup"><span data-stu-id="d246b-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d246b-119">Метаданные для отчета о действиях устройств с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="d246b-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="d246b-120">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="d246b-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="d246b-121">report</span><span class="sxs-lookup"><span data-stu-id="d246b-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d246b-122">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="d246b-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="d246b-123">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d246b-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="d246b-124">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="d246b-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="d246b-125">report</span><span class="sxs-lookup"><span data-stu-id="d246b-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d246b-126">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="d246b-126">Not yet documented.</span></span>|
|[<span data-ttu-id="d246b-127">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="d246b-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="d246b-128">report</span><span class="sxs-lookup"><span data-stu-id="d246b-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d246b-129">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="d246b-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="d246b-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="d246b-130">Properties</span></span>
|<span data-ttu-id="d246b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d246b-131">Property</span></span>|<span data-ttu-id="d246b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d246b-132">Type</span></span>|<span data-ttu-id="d246b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d246b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d246b-134">id</span><span class="sxs-lookup"><span data-stu-id="d246b-134">id</span></span>|<span data-ttu-id="d246b-135">String</span><span class="sxs-lookup"><span data-stu-id="d246b-135">String</span></span>|<span data-ttu-id="d246b-136">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="d246b-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d246b-137">Связи</span><span class="sxs-lookup"><span data-stu-id="d246b-137">Relationships</span></span>
<span data-ttu-id="d246b-138">Нет</span><span class="sxs-lookup"><span data-stu-id="d246b-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d246b-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d246b-139">JSON Representation</span></span>
<span data-ttu-id="d246b-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d246b-140">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="d246b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d246b-141">Example</span></span>

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