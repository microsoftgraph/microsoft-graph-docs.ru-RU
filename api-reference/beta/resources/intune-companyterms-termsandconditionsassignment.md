---
title: Тип ресурса termsAndConditionsAssignment
description: Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b6bff777bfaf093d1148a584cc8524069304b70
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788486"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="dcb75-104">Тип ресурса termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="dcb75-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb75-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcb75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb75-107">Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе.</span><span class="sxs-lookup"><span data-stu-id="dcb75-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="dcb75-108">Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.</span><span class="sxs-lookup"><span data-stu-id="dcb75-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="dcb75-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dcb75-109">Methods</span></span>
|<span data-ttu-id="dcb75-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dcb75-110">Method</span></span>|<span data-ttu-id="dcb75-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dcb75-111">Return Type</span></span>|<span data-ttu-id="dcb75-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb75-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dcb75-113">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="dcb75-114">Коллекция [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dcb75-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="dcb75-115">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcb75-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="dcb75-116">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="dcb75-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="dcb75-118">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcb75-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="dcb75-119">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="dcb75-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="dcb75-121">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcb75-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="dcb75-122">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="dcb75-123">Нет</span><span class="sxs-lookup"><span data-stu-id="dcb75-123">None</span></span>|<span data-ttu-id="dcb75-124">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcb75-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="dcb75-125">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="dcb75-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="dcb75-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="dcb75-127">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcb75-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dcb75-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcb75-128">Properties</span></span>
|<span data-ttu-id="dcb75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcb75-129">Property</span></span>|<span data-ttu-id="dcb75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb75-130">Type</span></span>|<span data-ttu-id="dcb75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb75-132">id</span><span class="sxs-lookup"><span data-stu-id="dcb75-132">id</span></span>|<span data-ttu-id="dcb75-133">String</span><span class="sxs-lookup"><span data-stu-id="dcb75-133">String</span></span>|<span data-ttu-id="dcb75-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="dcb75-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dcb75-135">target</span><span class="sxs-lookup"><span data-stu-id="dcb75-135">target</span></span>|[<span data-ttu-id="dcb75-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dcb75-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dcb75-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="dcb75-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcb75-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="dcb75-138">Relationships</span></span>
<span data-ttu-id="dcb75-139">Нет</span><span class="sxs-lookup"><span data-stu-id="dcb75-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcb75-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcb75-140">JSON Representation</span></span>
<span data-ttu-id="dcb75-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcb75-141">Here is a JSON representation of the resource.</span></span>
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





