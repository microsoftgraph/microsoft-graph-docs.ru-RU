---
title: Тип ресурса Граупполицикатегори
description: Сущность Category сохраняет категорию определения групповой политики
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b81a102bd5864d4f11f787e15bb2d709f0203cf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377193"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="cb715-103">Тип ресурса Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="cb715-103">groupPolicyCategory resource type</span></span>

<span data-ttu-id="cb715-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb715-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb715-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb715-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb715-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb715-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb715-107">Сущность Category сохраняет категорию определения групповой политики</span><span class="sxs-lookup"><span data-stu-id="cb715-107">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="cb715-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cb715-108">Methods</span></span>
|<span data-ttu-id="cb715-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cb715-109">Method</span></span>|<span data-ttu-id="cb715-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb715-110">Return Type</span></span>|<span data-ttu-id="cb715-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb715-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb715-112">Получение Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="cb715-112">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="cb715-113">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="cb715-113">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="cb715-114">Чтение свойств и связей объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="cb715-114">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="cb715-115">Обновление Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="cb715-115">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="cb715-116">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="cb715-116">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="cb715-117">Обновление свойств объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="cb715-117">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb715-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb715-118">Properties</span></span>
|<span data-ttu-id="cb715-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb715-119">Property</span></span>|<span data-ttu-id="cb715-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cb715-120">Type</span></span>|<span data-ttu-id="cb715-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cb715-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb715-122">displayName</span><span class="sxs-lookup"><span data-stu-id="cb715-122">displayName</span></span>|<span data-ttu-id="cb715-123">Строка</span><span class="sxs-lookup"><span data-stu-id="cb715-123">String</span></span>|<span data-ttu-id="cb715-124">Идентификатор строки отображаемого имени категории</span><span class="sxs-lookup"><span data-stu-id="cb715-124">The string id of the category's display name</span></span>|
|<span data-ttu-id="cb715-125">Корень</span><span class="sxs-lookup"><span data-stu-id="cb715-125">isRoot</span></span>|<span data-ttu-id="cb715-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb715-126">Boolean</span></span>|<span data-ttu-id="cb715-127">Определяет, является ли категория корневой категорией</span><span class="sxs-lookup"><span data-stu-id="cb715-127">Defines if the category is a root category</span></span>|
|<span data-ttu-id="cb715-128">id</span><span class="sxs-lookup"><span data-stu-id="cb715-128">id</span></span>|<span data-ttu-id="cb715-129">String</span><span class="sxs-lookup"><span data-stu-id="cb715-129">String</span></span>|<span data-ttu-id="cb715-130">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb715-130">Key of the entity.</span></span>|
|<span data-ttu-id="cb715-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb715-131">lastModifiedDateTime</span></span>|<span data-ttu-id="cb715-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb715-132">DateTimeOffset</span></span>|<span data-ttu-id="cb715-133">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb715-133">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb715-134">Связи</span><span class="sxs-lookup"><span data-stu-id="cb715-134">Relationships</span></span>
|<span data-ttu-id="cb715-135">Связь</span><span class="sxs-lookup"><span data-stu-id="cb715-135">Relationship</span></span>|<span data-ttu-id="cb715-136">Тип</span><span class="sxs-lookup"><span data-stu-id="cb715-136">Type</span></span>|<span data-ttu-id="cb715-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cb715-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb715-138">верхнего</span><span class="sxs-lookup"><span data-stu-id="cb715-138">parent</span></span>|[<span data-ttu-id="cb715-139">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="cb715-139">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="cb715-140">Родительская категория</span><span class="sxs-lookup"><span data-stu-id="cb715-140">The parent category</span></span>|
|<span data-ttu-id="cb715-141">children</span><span class="sxs-lookup"><span data-stu-id="cb715-141">children</span></span>|<span data-ttu-id="cb715-142">Коллекция [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="cb715-142">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="cb715-143">Категории дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="cb715-143">The children categories</span></span>|
|<span data-ttu-id="cb715-144">определения</span><span class="sxs-lookup"><span data-stu-id="cb715-144">definitions</span></span>|<span data-ttu-id="cb715-145">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cb715-145">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="cb715-146">Непосредственный дочерний элемент Граупполицидефинитион в категории</span><span class="sxs-lookup"><span data-stu-id="cb715-146">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="cb715-147">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="cb715-147">definitionFile</span></span>|[<span data-ttu-id="cb715-148">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="cb715-148">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="cb715-149">Идентификатор файла определения, из которого получена Категория</span><span class="sxs-lookup"><span data-stu-id="cb715-149">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb715-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb715-150">JSON Representation</span></span>
<span data-ttu-id="cb715-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb715-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



