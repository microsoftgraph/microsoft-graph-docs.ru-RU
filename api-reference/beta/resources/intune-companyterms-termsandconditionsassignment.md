---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb74dad5b75202d908b82b87e7fd66f7447aa826
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154917"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="e400a-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="e400a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e400a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e400a-106">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e400a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e400a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e400a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e400a-108">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="e400a-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="e400a-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="e400a-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="e400a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e400a-110">Methods</span></span>
|<span data-ttu-id="e400a-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e400a-111">Method</span></span>|<span data-ttu-id="e400a-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e400a-112">Return Type</span></span>|<span data-ttu-id="e400a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e400a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e400a-114">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="e400a-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="e400a-115">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e400a-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="e400a-116">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e400a-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="e400a-117">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="e400a-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e400a-119">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e400a-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="e400a-120">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="e400a-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e400a-122">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e400a-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="e400a-123">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="e400a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e400a-124">None</span></span>|<span data-ttu-id="e400a-125">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e400a-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="e400a-126">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="e400a-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e400a-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e400a-128">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e400a-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e400a-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e400a-129">Properties</span></span>
|<span data-ttu-id="e400a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e400a-130">Property</span></span>|<span data-ttu-id="e400a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e400a-131">Type</span></span>|<span data-ttu-id="e400a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e400a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e400a-133">id</span><span class="sxs-lookup"><span data-stu-id="e400a-133">id</span></span>|<span data-ttu-id="e400a-134">String</span><span class="sxs-lookup"><span data-stu-id="e400a-134">String</span></span>|<span data-ttu-id="e400a-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e400a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e400a-136">target</span><span class="sxs-lookup"><span data-stu-id="e400a-136">target</span></span>|[<span data-ttu-id="e400a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e400a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e400a-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="e400a-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e400a-139">Связи</span><span class="sxs-lookup"><span data-stu-id="e400a-139">Relationships</span></span>
<span data-ttu-id="e400a-140">Нет</span><span class="sxs-lookup"><span data-stu-id="e400a-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e400a-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e400a-141">JSON Representation</span></span>
<span data-ttu-id="e400a-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e400a-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




