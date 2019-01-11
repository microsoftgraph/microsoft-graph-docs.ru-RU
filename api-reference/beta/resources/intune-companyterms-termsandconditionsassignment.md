---
title: Тип ресурса termsAndConditionsAssignment
description: C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce4a1d77f3a3db1f1faee94c5435730515ff6af6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875063"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="d48ca-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="d48ca-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d48ca-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d48ca-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48ca-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d48ca-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d48ca-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d48ca-108">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="d48ca-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="d48ca-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="d48ca-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="d48ca-110">Методы</span><span class="sxs-lookup"><span data-stu-id="d48ca-110">Methods</span></span>
|<span data-ttu-id="d48ca-111">Метод</span><span class="sxs-lookup"><span data-stu-id="d48ca-111">Method</span></span>|<span data-ttu-id="d48ca-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d48ca-112">Return Type</span></span>|<span data-ttu-id="d48ca-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d48ca-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d48ca-114">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="d48ca-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="d48ca-115">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d48ca-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="d48ca-116">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48ca-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="d48ca-117">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="d48ca-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="d48ca-119">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48ca-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="d48ca-120">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="d48ca-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="d48ca-122">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48ca-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="d48ca-123">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="d48ca-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d48ca-124">None</span></span>|<span data-ttu-id="d48ca-125">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48ca-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="d48ca-126">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="d48ca-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d48ca-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="d48ca-128">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48ca-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d48ca-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="d48ca-129">Properties</span></span>
|<span data-ttu-id="d48ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d48ca-130">Property</span></span>|<span data-ttu-id="d48ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d48ca-131">Type</span></span>|<span data-ttu-id="d48ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d48ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d48ca-133">id</span><span class="sxs-lookup"><span data-stu-id="d48ca-133">id</span></span>|<span data-ttu-id="d48ca-134">String</span><span class="sxs-lookup"><span data-stu-id="d48ca-134">String</span></span>|<span data-ttu-id="d48ca-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d48ca-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d48ca-136">target</span><span class="sxs-lookup"><span data-stu-id="d48ca-136">target</span></span>|[<span data-ttu-id="d48ca-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d48ca-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d48ca-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="d48ca-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d48ca-139">Связи</span><span class="sxs-lookup"><span data-stu-id="d48ca-139">Relationships</span></span>
<span data-ttu-id="d48ca-140">Нет</span><span class="sxs-lookup"><span data-stu-id="d48ca-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d48ca-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d48ca-141">JSON Representation</span></span>
<span data-ttu-id="d48ca-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d48ca-142">Here is a JSON representation of the resource.</span></span>
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





