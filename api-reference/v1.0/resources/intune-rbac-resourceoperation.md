---
title: Тип ресурса resourceOperation
description: Описывает ресурс resourceOperation (Entity) API Microsoft Graph (REST), который поддерживает рабочие процессы Intune, связанные с управлением доступом на основе ролей (RBAC).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95083bb1a3eb9f3c6e98deadd005aa6ef700555a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441610"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="ce953-103">Тип ресурса resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-103">resourceOperation resource type</span></span>

<span data-ttu-id="ce953-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce953-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce953-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce953-106">Определяет операцию или действие, которые можно выполнять с ресурсом (или объектом) Intune.</span><span class="sxs-lookup"><span data-stu-id="ce953-106">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ce953-107">Распространенные операции — чтение, удаление, обновление и создание.</span><span class="sxs-lookup"><span data-stu-id="ce953-107">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="ce953-108">Они обеспечивают основные возможности управления базовым ресурсом Intune.</span><span class="sxs-lookup"><span data-stu-id="ce953-108">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ce953-109">В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="ce953-109">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ce953-110">Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.</span><span class="sxs-lookup"><span data-stu-id="ce953-110">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ce953-111">Операции с ресурсами невозможно изменить для встроенных ролей. Это определяет операцию или действие, которые можно выполнить с ресурсом (или объектом) Intune.</span><span class="sxs-lookup"><span data-stu-id="ce953-111">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ce953-112">Распространенные операции — получение, перечисление, обновление и создание.</span><span class="sxs-lookup"><span data-stu-id="ce953-112">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="ce953-113">Они обеспечивают основные возможности управления базовым ресурсом Intune.</span><span class="sxs-lookup"><span data-stu-id="ce953-113">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ce953-114">В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="ce953-114">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ce953-115">Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.</span><span class="sxs-lookup"><span data-stu-id="ce953-115">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ce953-116">Операции с ресурсами невозможно изменить для встроенных ролей.</span><span class="sxs-lookup"><span data-stu-id="ce953-116">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ce953-117">Методы</span><span class="sxs-lookup"><span data-stu-id="ce953-117">Methods</span></span>
|<span data-ttu-id="ce953-118">Метод</span><span class="sxs-lookup"><span data-stu-id="ce953-118">Method</span></span>|<span data-ttu-id="ce953-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce953-119">Return Type</span></span>|<span data-ttu-id="ce953-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ce953-120">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce953-121">Перечисление объектов resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-121">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="ce953-122">Коллекция объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ce953-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="ce953-123">Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ce953-123">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="ce953-124">Получение объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-124">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|<span data-ttu-id="ce953-125">[resourceOperation](../resources/intune-rbac-resourceoperation.md);</span><span class="sxs-lookup"><span data-stu-id="ce953-125">[resourceOperation](../resources/intune-rbac-resourceoperation.md)</span></span>|<span data-ttu-id="ce953-126">Чтение свойств и связей объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ce953-126">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ce953-127">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-127">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|<span data-ttu-id="ce953-128">[resourceOperation](../resources/intune-rbac-resourceoperation.md);</span><span class="sxs-lookup"><span data-stu-id="ce953-128">[resourceOperation](../resources/intune-rbac-resourceoperation.md)</span></span>|<span data-ttu-id="ce953-129">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ce953-129">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ce953-130">Удаление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-130">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="ce953-131">Нет</span><span class="sxs-lookup"><span data-stu-id="ce953-131">None</span></span>|<span data-ttu-id="ce953-132">Удаление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ce953-132">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="ce953-133">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-133">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="ce953-134">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ce953-134">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ce953-135">Обновление свойств объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ce953-135">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce953-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce953-136">Properties</span></span>
|<span data-ttu-id="ce953-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce953-137">Property</span></span>|<span data-ttu-id="ce953-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ce953-138">Type</span></span>|<span data-ttu-id="ce953-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ce953-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce953-140">id</span><span class="sxs-lookup"><span data-stu-id="ce953-140">id</span></span>|<span data-ttu-id="ce953-141">Строка</span><span class="sxs-lookup"><span data-stu-id="ce953-141">String</span></span>|<span data-ttu-id="ce953-142">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ce953-142">Key of the Resource Operation.</span></span> <span data-ttu-id="ce953-143">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ce953-143">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ce953-144">resourceName</span><span class="sxs-lookup"><span data-stu-id="ce953-144">resourceName</span></span>|<span data-ttu-id="ce953-145">String</span><span class="sxs-lookup"><span data-stu-id="ce953-145">String</span></span>|<span data-ttu-id="ce953-146">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="ce953-146">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ce953-147">actionName</span><span class="sxs-lookup"><span data-stu-id="ce953-147">actionName</span></span>|<span data-ttu-id="ce953-148">String</span><span class="sxs-lookup"><span data-stu-id="ce953-148">String</span></span>|<span data-ttu-id="ce953-149">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="ce953-149">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ce953-150">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="ce953-150">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ce953-151">description</span><span class="sxs-lookup"><span data-stu-id="ce953-151">description</span></span>|<span data-ttu-id="ce953-152">String</span><span class="sxs-lookup"><span data-stu-id="ce953-152">String</span></span>|<span data-ttu-id="ce953-153">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ce953-153">Description of the resource operation.</span></span> <span data-ttu-id="ce953-154">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ce953-154">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce953-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="ce953-155">Relationships</span></span>
<span data-ttu-id="ce953-156">Нет</span><span class="sxs-lookup"><span data-stu-id="ce953-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce953-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce953-157">JSON Representation</span></span>
<span data-ttu-id="ce953-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce953-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```







