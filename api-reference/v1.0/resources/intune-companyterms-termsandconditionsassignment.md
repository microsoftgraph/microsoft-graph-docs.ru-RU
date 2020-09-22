---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07c08866205338aa0d03f5fef4663935b6896b9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088610"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="7f6c4-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="7f6c4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f6c4-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f6c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f6c4-107">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="7f6c4-108">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="7f6c4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="7f6c4-109">Methods</span></span>
|<span data-ttu-id="7f6c4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="7f6c4-110">Method</span></span>|<span data-ttu-id="7f6c4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f6c4-111">Return Type</span></span>|<span data-ttu-id="7f6c4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7f6c4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f6c4-113">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="7f6c4-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="7f6c4-114">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7f6c4-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="7f6c4-115">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f6c4-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="7f6c4-116">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="7f6c4-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7f6c4-118">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f6c4-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7f6c4-119">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="7f6c4-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7f6c4-121">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f6c4-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7f6c4-122">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="7f6c4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7f6c4-123">None</span></span>|<span data-ttu-id="7f6c4-124">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f6c4-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="7f6c4-125">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="7f6c4-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f6c4-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7f6c4-127">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f6c4-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f6c4-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f6c4-128">Properties</span></span>
|<span data-ttu-id="7f6c4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f6c4-129">Property</span></span>|<span data-ttu-id="7f6c4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f6c4-130">Type</span></span>|<span data-ttu-id="7f6c4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f6c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6c4-132">id</span><span class="sxs-lookup"><span data-stu-id="7f6c4-132">id</span></span>|<span data-ttu-id="7f6c4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7f6c4-133">String</span></span>|<span data-ttu-id="7f6c4-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7f6c4-135">target</span><span class="sxs-lookup"><span data-stu-id="7f6c4-135">target</span></span>|[<span data-ttu-id="7f6c4-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f6c4-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f6c4-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f6c4-138">Связи</span><span class="sxs-lookup"><span data-stu-id="7f6c4-138">Relationships</span></span>
<span data-ttu-id="7f6c4-139">Нет</span><span class="sxs-lookup"><span data-stu-id="7f6c4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f6c4-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f6c4-140">JSON Representation</span></span>
<span data-ttu-id="7f6c4-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f6c4-141">Here is a JSON representation of the resource.</span></span>
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









