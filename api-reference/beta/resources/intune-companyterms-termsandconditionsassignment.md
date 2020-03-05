---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 21be6ea2550f83210a2760d306bd3988ad17198e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487594"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="598a8-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="598a8-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="598a8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="598a8-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="598a8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="598a8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="598a8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="598a8-108">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="598a8-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="598a8-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="598a8-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="598a8-110">Методы</span><span class="sxs-lookup"><span data-stu-id="598a8-110">Methods</span></span>
|<span data-ttu-id="598a8-111">Метод</span><span class="sxs-lookup"><span data-stu-id="598a8-111">Method</span></span>|<span data-ttu-id="598a8-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="598a8-112">Return Type</span></span>|<span data-ttu-id="598a8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="598a8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="598a8-114">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="598a8-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="598a8-115">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="598a8-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="598a8-116">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="598a8-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="598a8-117">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="598a8-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="598a8-119">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="598a8-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="598a8-120">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="598a8-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="598a8-122">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="598a8-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="598a8-123">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="598a8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="598a8-124">None</span></span>|<span data-ttu-id="598a8-125">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="598a8-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="598a8-126">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="598a8-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="598a8-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="598a8-128">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="598a8-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="598a8-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="598a8-129">Properties</span></span>
|<span data-ttu-id="598a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="598a8-130">Property</span></span>|<span data-ttu-id="598a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="598a8-131">Type</span></span>|<span data-ttu-id="598a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="598a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598a8-133">id</span><span class="sxs-lookup"><span data-stu-id="598a8-133">id</span></span>|<span data-ttu-id="598a8-134">String</span><span class="sxs-lookup"><span data-stu-id="598a8-134">String</span></span>|<span data-ttu-id="598a8-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="598a8-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="598a8-136">target</span><span class="sxs-lookup"><span data-stu-id="598a8-136">target</span></span>|[<span data-ttu-id="598a8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="598a8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="598a8-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="598a8-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="598a8-139">Связи</span><span class="sxs-lookup"><span data-stu-id="598a8-139">Relationships</span></span>
<span data-ttu-id="598a8-140">Нет</span><span class="sxs-lookup"><span data-stu-id="598a8-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="598a8-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="598a8-141">JSON Representation</span></span>
<span data-ttu-id="598a8-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="598a8-142">Here is a JSON representation of the resource.</span></span>
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



