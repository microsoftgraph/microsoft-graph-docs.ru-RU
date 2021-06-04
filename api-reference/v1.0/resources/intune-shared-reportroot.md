---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe26bc7b5effb24fb0855da6d84b464f36de4927
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732713"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="1b6cf-103">Тип ресурса reportRoot</span><span class="sxs-lookup"><span data-stu-id="1b6cf-103">reportRoot resource type</span></span>

<span data-ttu-id="1b6cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b6cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b6cf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b6cf-106">Ресурс, представляющий экземпляр отчетов журнала.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-106">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="1b6cf-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1b6cf-107">Methods</span></span>
|<span data-ttu-id="1b6cf-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1b6cf-108">Method</span></span>|<span data-ttu-id="1b6cf-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b6cf-109">Return Type</span></span>|<span data-ttu-id="1b6cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6cf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b6cf-111">Получение объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="1b6cf-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="1b6cf-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="1b6cf-112">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="1b6cf-113">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1b6cf-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="1b6cf-114">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="1b6cf-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="1b6cf-115">reportRoot</span><span class="sxs-lookup"><span data-stu-id="1b6cf-115">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="1b6cf-116">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1b6cf-116">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="1b6cf-117">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="1b6cf-117">**Device configuration**</span></span>|
|[<span data-ttu-id="1b6cf-118">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="1b6cf-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="1b6cf-119">report</span><span class="sxs-lookup"><span data-stu-id="1b6cf-119">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1b6cf-120">Метаданные для отчета о действиях устройств с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="1b6cf-120">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="1b6cf-121">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="1b6cf-121">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="1b6cf-122">report</span><span class="sxs-lookup"><span data-stu-id="1b6cf-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1b6cf-123">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="1b6cf-123">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="1b6cf-124">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="1b6cf-124">**Troubleshooting**</span></span>|
|[<span data-ttu-id="1b6cf-125">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="1b6cf-125">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="1b6cf-126">report</span><span class="sxs-lookup"><span data-stu-id="1b6cf-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1b6cf-127">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-127">Not yet documented.</span></span>|
|[<span data-ttu-id="1b6cf-128">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="1b6cf-128">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="1b6cf-129">report</span><span class="sxs-lookup"><span data-stu-id="1b6cf-129">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="1b6cf-130">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-130">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="1b6cf-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b6cf-131">Properties</span></span>
|<span data-ttu-id="1b6cf-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b6cf-132">Property</span></span>|<span data-ttu-id="1b6cf-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1b6cf-133">Type</span></span>|<span data-ttu-id="1b6cf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6cf-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b6cf-135">id</span><span class="sxs-lookup"><span data-stu-id="1b6cf-135">id</span></span>|<span data-ttu-id="1b6cf-136">String</span><span class="sxs-lookup"><span data-stu-id="1b6cf-136">String</span></span>|<span data-ttu-id="1b6cf-137">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-137">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b6cf-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="1b6cf-138">Relationships</span></span>
<span data-ttu-id="1b6cf-139">Нет</span><span class="sxs-lookup"><span data-stu-id="1b6cf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b6cf-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b6cf-140">JSON Representation</span></span>
<span data-ttu-id="1b6cf-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b6cf-141">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="1b6cf-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1b6cf-142">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```






