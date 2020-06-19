---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 615bb6710f2acb82519cdbc87a0f8628f178b29e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793488"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="9f134-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="9f134-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f134-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f134-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f134-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f134-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f134-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f134-108">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="9f134-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="9f134-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="9f134-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="9f134-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9f134-110">Methods</span></span>
|<span data-ttu-id="9f134-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9f134-111">Method</span></span>|<span data-ttu-id="9f134-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f134-112">Return Type</span></span>|<span data-ttu-id="9f134-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9f134-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f134-114">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="9f134-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="9f134-115">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9f134-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="9f134-116">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f134-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="9f134-117">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="9f134-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9f134-119">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f134-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="9f134-120">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="9f134-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9f134-122">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f134-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="9f134-123">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="9f134-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9f134-124">None</span></span>|<span data-ttu-id="9f134-125">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f134-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="9f134-126">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="9f134-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9f134-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9f134-128">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f134-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f134-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f134-129">Properties</span></span>
|<span data-ttu-id="9f134-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f134-130">Property</span></span>|<span data-ttu-id="9f134-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f134-131">Type</span></span>|<span data-ttu-id="9f134-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f134-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f134-133">id</span><span class="sxs-lookup"><span data-stu-id="9f134-133">id</span></span>|<span data-ttu-id="9f134-134">String</span><span class="sxs-lookup"><span data-stu-id="9f134-134">String</span></span>|<span data-ttu-id="9f134-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9f134-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9f134-136">target</span><span class="sxs-lookup"><span data-stu-id="9f134-136">target</span></span>|[<span data-ttu-id="9f134-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f134-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f134-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="9f134-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f134-139">Связи</span><span class="sxs-lookup"><span data-stu-id="9f134-139">Relationships</span></span>
<span data-ttu-id="9f134-140">Нет</span><span class="sxs-lookup"><span data-stu-id="9f134-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f134-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f134-141">JSON Representation</span></span>
<span data-ttu-id="9f134-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f134-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



