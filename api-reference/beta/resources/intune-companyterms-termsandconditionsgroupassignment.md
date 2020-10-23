---
title: Тип ресурса Термсандкондитионсграупассигнмент
description: Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (T&C) для данной группы. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9236ee34c07836e97fca89636f128b12dbb7d576
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726516"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="c42e3-104">Тип ресурса Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-104">termsAndConditionsGroupAssignment resource type</span></span>

<span data-ttu-id="c42e3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c42e3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c42e3-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c42e3-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c42e3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c42e3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c42e3-108">Объект Термсандкондитионсграупассигнмент представляет назначение определенной политики условий (T&C) для данной группы.</span><span class="sxs-lookup"><span data-stu-id="c42e3-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="c42e3-109">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="c42e3-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="c42e3-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c42e3-110">Methods</span></span>
|<span data-ttu-id="c42e3-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c42e3-111">Method</span></span>|<span data-ttu-id="c42e3-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c42e3-112">Return Type</span></span>|<span data-ttu-id="c42e3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c42e3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c42e3-114">Список Термсандкондитионсграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="c42e3-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="c42e3-115">Коллекция [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c42e3-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="c42e3-116">Список свойств и связей объектов [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c42e3-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="c42e3-117">Получение Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="c42e3-118">термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="c42e3-119">Чтение свойств и связей объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c42e3-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="c42e3-120">Создание Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="c42e3-121">термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="c42e3-122">Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c42e3-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="c42e3-123">Удаление Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="c42e3-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c42e3-124">None</span></span>|<span data-ttu-id="c42e3-125">Удаляет объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c42e3-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="c42e3-126">Обновление Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="c42e3-127">термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="c42e3-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="c42e3-128">Обновление свойств объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c42e3-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c42e3-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="c42e3-129">Properties</span></span>
|<span data-ttu-id="c42e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c42e3-130">Property</span></span>|<span data-ttu-id="c42e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c42e3-131">Type</span></span>|<span data-ttu-id="c42e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c42e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c42e3-133">id</span><span class="sxs-lookup"><span data-stu-id="c42e3-133">id</span></span>|<span data-ttu-id="c42e3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c42e3-134">String</span></span>|<span data-ttu-id="c42e3-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c42e3-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c42e3-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="c42e3-136">targetGroupId</span></span>|<span data-ttu-id="c42e3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c42e3-137">String</span></span>|<span data-ttu-id="c42e3-138">Уникальный идентификатор группы, которой назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="c42e3-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c42e3-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c42e3-139">Relationships</span></span>
|<span data-ttu-id="c42e3-140">Связь</span><span class="sxs-lookup"><span data-stu-id="c42e3-140">Relationship</span></span>|<span data-ttu-id="c42e3-141">Тип</span><span class="sxs-lookup"><span data-stu-id="c42e3-141">Type</span></span>|<span data-ttu-id="c42e3-142">Описание</span><span class="sxs-lookup"><span data-stu-id="c42e3-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c42e3-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c42e3-143">termsAndConditions</span></span>|[<span data-ttu-id="c42e3-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c42e3-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="c42e3-145">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="c42e3-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c42e3-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c42e3-146">JSON Representation</span></span>
<span data-ttu-id="c42e3-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c42e3-147">Here is a JSON representation of the resource.</span></span>
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





