---
title: Тип ресурса termsAndConditionsAssignment
description: C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7fca6763ec7214b2dfd111996e965f9e9c995ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979483"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="a973b-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="a973b-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a973b-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a973b-106">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="a973b-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="a973b-107">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="a973b-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="a973b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a973b-108">Methods</span></span>
|<span data-ttu-id="a973b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a973b-109">Method</span></span>|<span data-ttu-id="a973b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a973b-110">Return Type</span></span>|<span data-ttu-id="a973b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a973b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a973b-112">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="a973b-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="a973b-113">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a973b-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="a973b-114">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a973b-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="a973b-115">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="a973b-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a973b-117">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a973b-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="a973b-118">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="a973b-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a973b-120">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a973b-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="a973b-121">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="a973b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a973b-122">None</span></span>|<span data-ttu-id="a973b-123">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a973b-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="a973b-124">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="a973b-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a973b-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="a973b-126">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a973b-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a973b-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="a973b-127">Properties</span></span>
|<span data-ttu-id="a973b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a973b-128">Property</span></span>|<span data-ttu-id="a973b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a973b-129">Type</span></span>|<span data-ttu-id="a973b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a973b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a973b-131">id</span><span class="sxs-lookup"><span data-stu-id="a973b-131">id</span></span>|<span data-ttu-id="a973b-132">String</span><span class="sxs-lookup"><span data-stu-id="a973b-132">String</span></span>|<span data-ttu-id="a973b-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="a973b-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a973b-134">target</span><span class="sxs-lookup"><span data-stu-id="a973b-134">target</span></span>|[<span data-ttu-id="a973b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a973b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a973b-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="a973b-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a973b-137">Связи</span><span class="sxs-lookup"><span data-stu-id="a973b-137">Relationships</span></span>
<span data-ttu-id="a973b-138">Нет</span><span class="sxs-lookup"><span data-stu-id="a973b-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a973b-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a973b-139">JSON Representation</span></span>
<span data-ttu-id="a973b-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a973b-140">Here is a JSON representation of the resource.</span></span>
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



