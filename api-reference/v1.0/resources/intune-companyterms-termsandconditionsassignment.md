---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b11f96cb6c8b1062c25e194ab8e3d96ea7c1deeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031985"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="aeac9-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="aeac9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aeac9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeac9-106">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="aeac9-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="aeac9-107">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="aeac9-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="aeac9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="aeac9-108">Methods</span></span>
|<span data-ttu-id="aeac9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="aeac9-109">Method</span></span>|<span data-ttu-id="aeac9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aeac9-110">Return Type</span></span>|<span data-ttu-id="aeac9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aeac9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aeac9-112">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="aeac9-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="aeac9-113">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aeac9-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="aeac9-114">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aeac9-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="aeac9-115">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="aeac9-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="aeac9-117">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aeac9-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="aeac9-118">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="aeac9-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="aeac9-120">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aeac9-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="aeac9-121">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="aeac9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="aeac9-122">None</span></span>|<span data-ttu-id="aeac9-123">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aeac9-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="aeac9-124">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="aeac9-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="aeac9-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="aeac9-126">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aeac9-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aeac9-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeac9-127">Properties</span></span>
|<span data-ttu-id="aeac9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeac9-128">Property</span></span>|<span data-ttu-id="aeac9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="aeac9-129">Type</span></span>|<span data-ttu-id="aeac9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="aeac9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeac9-131">id</span><span class="sxs-lookup"><span data-stu-id="aeac9-131">id</span></span>|<span data-ttu-id="aeac9-132">String</span><span class="sxs-lookup"><span data-stu-id="aeac9-132">String</span></span>|<span data-ttu-id="aeac9-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="aeac9-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="aeac9-134">target</span><span class="sxs-lookup"><span data-stu-id="aeac9-134">target</span></span>|[<span data-ttu-id="aeac9-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aeac9-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aeac9-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="aeac9-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeac9-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="aeac9-137">Relationships</span></span>
<span data-ttu-id="aeac9-138">Нет</span><span class="sxs-lookup"><span data-stu-id="aeac9-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aeac9-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aeac9-139">JSON Representation</span></span>
<span data-ttu-id="aeac9-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeac9-140">Here is a JSON representation of the resource.</span></span>
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



