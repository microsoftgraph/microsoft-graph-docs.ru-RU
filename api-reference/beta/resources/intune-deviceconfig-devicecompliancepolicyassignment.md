---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
author: tfitzmac
ms.openlocfilehash: 9e589cb6191a7d8ca7406125419bcfae03304ade
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310677"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="2fa28-103">Тип ресурса deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="2fa28-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2fa28-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fa28-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fa28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fa28-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2fa28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fa28-107">Назначение политики соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="2fa28-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="2fa28-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2fa28-108">Methods</span></span>
|<span data-ttu-id="2fa28-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2fa28-109">Method</span></span>|<span data-ttu-id="2fa28-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2fa28-110">Return Type</span></span>|<span data-ttu-id="2fa28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa28-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fa28-112">Список объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="2fa28-113">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2fa28-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="2fa28-114">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa28-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="2fa28-115">Получение объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="2fa28-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="2fa28-117">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa28-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="2fa28-118">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="2fa28-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="2fa28-120">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa28-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="2fa28-121">Удаление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="2fa28-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2fa28-122">None</span></span>|<span data-ttu-id="2fa28-123">Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa28-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="2fa28-124">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="2fa28-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2fa28-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="2fa28-126">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa28-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2fa28-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fa28-127">Properties</span></span>
|<span data-ttu-id="2fa28-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fa28-128">Property</span></span>|<span data-ttu-id="2fa28-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2fa28-129">Type</span></span>|<span data-ttu-id="2fa28-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa28-131">id</span><span class="sxs-lookup"><span data-stu-id="2fa28-131">id</span></span>|<span data-ttu-id="2fa28-132">Строка</span><span class="sxs-lookup"><span data-stu-id="2fa28-132">String</span></span>|<span data-ttu-id="2fa28-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2fa28-133">Key of the entity.</span></span>|
|<span data-ttu-id="2fa28-134">target</span><span class="sxs-lookup"><span data-stu-id="2fa28-134">target</span></span>|[<span data-ttu-id="2fa28-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2fa28-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2fa28-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="2fa28-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fa28-137">Связи</span><span class="sxs-lookup"><span data-stu-id="2fa28-137">Relationships</span></span>
<span data-ttu-id="2fa28-138">Нет</span><span class="sxs-lookup"><span data-stu-id="2fa28-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fa28-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fa28-139">JSON Representation</span></span>
<span data-ttu-id="2fa28-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fa28-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





