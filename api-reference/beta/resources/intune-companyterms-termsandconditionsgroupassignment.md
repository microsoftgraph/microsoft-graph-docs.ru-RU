---
title: Тип ресурса termsAndConditionsGroupAssignment
description: Сущность termsAndConditionsGroupAssignment представляет назначение присвоенное сроками и условиями (T&C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418577"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="b5a28-104">Тип ресурса termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="b5a28-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5a28-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5a28-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5a28-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5a28-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5a28-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5a28-108">Сущность termsAndConditionsGroupAssignment представляет назначение присвоенное сроками и условиями (T&C) политики к определенной группе.</span><span class="sxs-lookup"><span data-stu-id="b5a28-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="b5a28-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="b5a28-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="b5a28-110">Методы</span><span class="sxs-lookup"><span data-stu-id="b5a28-110">Methods</span></span>
|<span data-ttu-id="b5a28-111">Метод</span><span class="sxs-lookup"><span data-stu-id="b5a28-111">Method</span></span>|<span data-ttu-id="b5a28-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5a28-112">Return Type</span></span>|<span data-ttu-id="b5a28-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a28-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5a28-114">Список termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="b5a28-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="b5a28-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b5a28-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="b5a28-116">Свойства списка и связей объектов [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a28-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="b5a28-117">Получение termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="b5a28-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="b5a28-119">Чтение свойства и связи объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a28-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="b5a28-120">Создание termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="b5a28-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="b5a28-122">Создание нового объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a28-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="b5a28-123">Удаление termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="b5a28-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b5a28-124">None</span></span>|<span data-ttu-id="b5a28-125">Удаляет [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b5a28-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="b5a28-126">Обновление termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="b5a28-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b5a28-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="b5a28-128">Обновление свойства объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a28-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5a28-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5a28-129">Properties</span></span>
|<span data-ttu-id="b5a28-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5a28-130">Property</span></span>|<span data-ttu-id="b5a28-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b5a28-131">Type</span></span>|<span data-ttu-id="b5a28-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a28-133">id</span><span class="sxs-lookup"><span data-stu-id="b5a28-133">id</span></span>|<span data-ttu-id="b5a28-134">String</span><span class="sxs-lookup"><span data-stu-id="b5a28-134">String</span></span>|<span data-ttu-id="b5a28-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b5a28-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b5a28-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b5a28-136">targetGroupId</span></span>|<span data-ttu-id="b5a28-137">String</span><span class="sxs-lookup"><span data-stu-id="b5a28-137">String</span></span>|<span data-ttu-id="b5a28-138">Уникальный идентификатор группы, которая назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="b5a28-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5a28-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5a28-139">Relationships</span></span>
|<span data-ttu-id="b5a28-140">Связь</span><span class="sxs-lookup"><span data-stu-id="b5a28-140">Relationship</span></span>|<span data-ttu-id="b5a28-141">Тип</span><span class="sxs-lookup"><span data-stu-id="b5a28-141">Type</span></span>|<span data-ttu-id="b5a28-142">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a28-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a28-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b5a28-143">termsAndConditions</span></span>|[<span data-ttu-id="b5a28-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b5a28-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="b5a28-145">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="b5a28-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5a28-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5a28-146">JSON Representation</span></span>
<span data-ttu-id="b5a28-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5a28-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




