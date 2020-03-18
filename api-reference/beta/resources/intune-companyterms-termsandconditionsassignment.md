---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea848f1e253f3cce0e204d55fbe61f7d54abdc86
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797264"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="ff3cf-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="ff3cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff3cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff3cf-107">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="ff3cf-108">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="ff3cf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ff3cf-109">Methods</span></span>
|<span data-ttu-id="ff3cf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ff3cf-110">Method</span></span>|<span data-ttu-id="ff3cf-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff3cf-111">Return Type</span></span>|<span data-ttu-id="ff3cf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff3cf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff3cf-113">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="ff3cf-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="ff3cf-114">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ff3cf-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="ff3cf-115">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3cf-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="ff3cf-116">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="ff3cf-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ff3cf-118">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3cf-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="ff3cf-119">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="ff3cf-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ff3cf-121">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3cf-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="ff3cf-122">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="ff3cf-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ff3cf-123">None</span></span>|<span data-ttu-id="ff3cf-124">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3cf-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="ff3cf-125">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="ff3cf-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3cf-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="ff3cf-127">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3cf-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff3cf-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff3cf-128">Properties</span></span>
|<span data-ttu-id="ff3cf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff3cf-129">Property</span></span>|<span data-ttu-id="ff3cf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ff3cf-130">Type</span></span>|<span data-ttu-id="ff3cf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ff3cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3cf-132">id</span><span class="sxs-lookup"><span data-stu-id="ff3cf-132">id</span></span>|<span data-ttu-id="ff3cf-133">String</span><span class="sxs-lookup"><span data-stu-id="ff3cf-133">String</span></span>|<span data-ttu-id="ff3cf-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ff3cf-135">target</span><span class="sxs-lookup"><span data-stu-id="ff3cf-135">target</span></span>|[<span data-ttu-id="ff3cf-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff3cf-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff3cf-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff3cf-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ff3cf-138">Relationships</span></span>
<span data-ttu-id="ff3cf-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ff3cf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff3cf-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff3cf-140">JSON Representation</span></span>
<span data-ttu-id="ff3cf-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff3cf-141">Here is a JSON representation of the resource.</span></span>
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



