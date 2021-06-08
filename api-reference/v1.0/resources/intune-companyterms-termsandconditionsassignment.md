---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead01aac6a0ae8b297b6c013ce2a2a3b4e421956
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758927"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="60503-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="60503-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60503-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60503-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60503-107">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="60503-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="60503-108">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="60503-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="60503-109">Методы</span><span class="sxs-lookup"><span data-stu-id="60503-109">Methods</span></span>
|<span data-ttu-id="60503-110">Метод</span><span class="sxs-lookup"><span data-stu-id="60503-110">Method</span></span>|<span data-ttu-id="60503-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60503-111">Return Type</span></span>|<span data-ttu-id="60503-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60503-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60503-113">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="60503-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="60503-114">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="60503-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="60503-115">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60503-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="60503-116">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="60503-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60503-118">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60503-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="60503-119">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="60503-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60503-121">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60503-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="60503-122">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="60503-123">Нет</span><span class="sxs-lookup"><span data-stu-id="60503-123">None</span></span>|<span data-ttu-id="60503-124">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60503-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="60503-125">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="60503-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60503-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60503-127">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60503-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60503-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="60503-128">Properties</span></span>
|<span data-ttu-id="60503-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="60503-129">Property</span></span>|<span data-ttu-id="60503-130">Тип</span><span class="sxs-lookup"><span data-stu-id="60503-130">Type</span></span>|<span data-ttu-id="60503-131">Описание</span><span class="sxs-lookup"><span data-stu-id="60503-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60503-132">id</span><span class="sxs-lookup"><span data-stu-id="60503-132">id</span></span>|<span data-ttu-id="60503-133">String</span><span class="sxs-lookup"><span data-stu-id="60503-133">String</span></span>|<span data-ttu-id="60503-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="60503-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="60503-135">target</span><span class="sxs-lookup"><span data-stu-id="60503-135">target</span></span>|[<span data-ttu-id="60503-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="60503-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="60503-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="60503-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60503-138">Связи</span><span class="sxs-lookup"><span data-stu-id="60503-138">Relationships</span></span>
<span data-ttu-id="60503-139">Нет</span><span class="sxs-lookup"><span data-stu-id="60503-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60503-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60503-140">JSON Representation</span></span>
<span data-ttu-id="60503-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60503-141">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




