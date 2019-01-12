---
title: Тип ресурса termsAndConditionsGroupAssignment
description: C) политики к определенной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3efd219e175743afdca35d1b4348de0c6f571540
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954115"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="07995-104">Тип ресурса termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="07995-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07995-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07995-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07995-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07995-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07995-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07995-108">Сущность termsAndConditionsGroupAssignment представляет назначения сроками и условиями (T & C) групповой политики для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="07995-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="07995-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="07995-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="07995-110">Методы</span><span class="sxs-lookup"><span data-stu-id="07995-110">Methods</span></span>
|<span data-ttu-id="07995-111">Метод</span><span class="sxs-lookup"><span data-stu-id="07995-111">Method</span></span>|<span data-ttu-id="07995-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="07995-112">Return Type</span></span>|<span data-ttu-id="07995-113">Описание</span><span class="sxs-lookup"><span data-stu-id="07995-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07995-114">Список termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="07995-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="07995-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="07995-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="07995-116">Свойства списка и связей объектов [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07995-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="07995-117">Получение termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="07995-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="07995-119">Чтение свойства и связи объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07995-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="07995-120">Создание termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="07995-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="07995-122">Создание нового объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07995-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="07995-123">Удаление termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="07995-124">Нет</span><span class="sxs-lookup"><span data-stu-id="07995-124">None</span></span>|<span data-ttu-id="07995-125">Удаляет [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07995-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="07995-126">Обновление termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="07995-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07995-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="07995-128">Обновление свойства объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07995-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07995-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="07995-129">Properties</span></span>
|<span data-ttu-id="07995-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07995-130">Property</span></span>|<span data-ttu-id="07995-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07995-131">Type</span></span>|<span data-ttu-id="07995-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07995-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07995-133">id</span><span class="sxs-lookup"><span data-stu-id="07995-133">id</span></span>|<span data-ttu-id="07995-134">String</span><span class="sxs-lookup"><span data-stu-id="07995-134">String</span></span>|<span data-ttu-id="07995-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="07995-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="07995-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="07995-136">targetGroupId</span></span>|<span data-ttu-id="07995-137">Строка</span><span class="sxs-lookup"><span data-stu-id="07995-137">String</span></span>|<span data-ttu-id="07995-138">Уникальный идентификатор группы, которая назначена политика T & C.</span><span class="sxs-lookup"><span data-stu-id="07995-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07995-139">Связи</span><span class="sxs-lookup"><span data-stu-id="07995-139">Relationships</span></span>
|<span data-ttu-id="07995-140">Связь</span><span class="sxs-lookup"><span data-stu-id="07995-140">Relationship</span></span>|<span data-ttu-id="07995-141">Тип</span><span class="sxs-lookup"><span data-stu-id="07995-141">Type</span></span>|<span data-ttu-id="07995-142">Описание</span><span class="sxs-lookup"><span data-stu-id="07995-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07995-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="07995-143">termsAndConditions</span></span>|[<span data-ttu-id="07995-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="07995-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="07995-145">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="07995-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07995-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07995-146">JSON Representation</span></span>
<span data-ttu-id="07995-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07995-147">Here is a JSON representation of the resource.</span></span>
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





