---
title: Тип ресурса termsAndConditionsAssignment
description: C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75c9946cead03b2d7c0630c29a9b28c47ac1b269
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919808"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="162e5-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="162e5-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="162e5-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162e5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="162e5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="162e5-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="162e5-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="162e5-108">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="162e5-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="162e5-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="162e5-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="162e5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="162e5-110">Methods</span></span>
|<span data-ttu-id="162e5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="162e5-111">Method</span></span>|<span data-ttu-id="162e5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="162e5-112">Return Type</span></span>|<span data-ttu-id="162e5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="162e5-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="162e5-114">Список termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="162e5-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="162e5-115">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="162e5-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="162e5-116">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="162e5-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="162e5-117">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="162e5-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="162e5-119">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="162e5-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="162e5-120">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="162e5-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="162e5-122">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="162e5-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="162e5-123">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="162e5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="162e5-124">None</span></span>|<span data-ttu-id="162e5-125">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="162e5-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="162e5-126">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="162e5-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="162e5-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="162e5-128">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="162e5-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="162e5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="162e5-129">Properties</span></span>
|<span data-ttu-id="162e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="162e5-130">Property</span></span>|<span data-ttu-id="162e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="162e5-131">Type</span></span>|<span data-ttu-id="162e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="162e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162e5-133">id</span><span class="sxs-lookup"><span data-stu-id="162e5-133">id</span></span>|<span data-ttu-id="162e5-134">String</span><span class="sxs-lookup"><span data-stu-id="162e5-134">String</span></span>|<span data-ttu-id="162e5-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="162e5-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="162e5-136">target</span><span class="sxs-lookup"><span data-stu-id="162e5-136">target</span></span>|[<span data-ttu-id="162e5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="162e5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="162e5-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="162e5-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="162e5-139">Связи</span><span class="sxs-lookup"><span data-stu-id="162e5-139">Relationships</span></span>
<span data-ttu-id="162e5-140">Нет</span><span class="sxs-lookup"><span data-stu-id="162e5-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="162e5-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="162e5-141">JSON Representation</span></span>
<span data-ttu-id="162e5-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="162e5-142">Here is a JSON representation of the resource.</span></span>
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





