---
title: Тип ресурса termsAndConditionsAssignment
description: C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
ms.openlocfilehash: 848998e59f214fc679aba7c27a2a529be05c8adc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027181"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="74ac6-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="74ac6-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74ac6-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74ac6-106">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="74ac6-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="74ac6-107">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="74ac6-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="74ac6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="74ac6-108">Methods</span></span>
|<span data-ttu-id="74ac6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="74ac6-109">Method</span></span>|<span data-ttu-id="74ac6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74ac6-110">Return Type</span></span>|<span data-ttu-id="74ac6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74ac6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74ac6-112">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="74ac6-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="74ac6-113">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="74ac6-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="74ac6-114">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74ac6-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="74ac6-115">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="74ac6-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="74ac6-117">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74ac6-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="74ac6-118">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="74ac6-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="74ac6-120">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74ac6-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="74ac6-121">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="74ac6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="74ac6-122">None</span></span>|<span data-ttu-id="74ac6-123">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74ac6-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="74ac6-124">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="74ac6-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="74ac6-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="74ac6-126">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74ac6-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74ac6-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="74ac6-127">Properties</span></span>
|<span data-ttu-id="74ac6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ac6-128">Property</span></span>|<span data-ttu-id="74ac6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="74ac6-129">Type</span></span>|<span data-ttu-id="74ac6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="74ac6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ac6-131">id</span><span class="sxs-lookup"><span data-stu-id="74ac6-131">id</span></span>|<span data-ttu-id="74ac6-132">String</span><span class="sxs-lookup"><span data-stu-id="74ac6-132">String</span></span>|<span data-ttu-id="74ac6-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="74ac6-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="74ac6-134">target</span><span class="sxs-lookup"><span data-stu-id="74ac6-134">target</span></span>|[<span data-ttu-id="74ac6-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="74ac6-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="74ac6-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="74ac6-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74ac6-137">Связи</span><span class="sxs-lookup"><span data-stu-id="74ac6-137">Relationships</span></span>
<span data-ttu-id="74ac6-138">Нет</span><span class="sxs-lookup"><span data-stu-id="74ac6-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74ac6-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74ac6-139">JSON Representation</span></span>
<span data-ttu-id="74ac6-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74ac6-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



