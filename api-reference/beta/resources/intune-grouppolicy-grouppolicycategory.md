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
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="f2fc5-103">Тип ресурса Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="f2fc5-103">groupPolicyCategory resource type</span></span>

<span data-ttu-id="f2fc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2fc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2fc5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2fc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2fc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2fc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2fc5-107">Сущность Category сохраняет категорию определения групповой политики</span><span class="sxs-lookup"><span data-stu-id="f2fc5-107">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="f2fc5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f2fc5-108">Methods</span></span>
|<span data-ttu-id="f2fc5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f2fc5-109">Method</span></span>|<span data-ttu-id="f2fc5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2fc5-110">Return Type</span></span>|<span data-ttu-id="f2fc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2fc5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2fc5-112">Получение Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="f2fc5-112">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="f2fc5-113">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="f2fc5-113">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="f2fc5-114">Чтение свойств и связей объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f2fc5-114">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="f2fc5-115">Обновление Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="f2fc5-115">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="f2fc5-116">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="f2fc5-116">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="f2fc5-117">Обновление свойств объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f2fc5-117">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2fc5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2fc5-118">Properties</span></span>
|<span data-ttu-id="f2fc5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2fc5-119">Property</span></span>|<span data-ttu-id="f2fc5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f2fc5-120">Type</span></span>|<span data-ttu-id="f2fc5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f2fc5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fc5-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f2fc5-122">displayName</span></span>|<span data-ttu-id="f2fc5-123">Строка</span><span class="sxs-lookup"><span data-stu-id="f2fc5-123">String</span></span>|<span data-ttu-id="f2fc5-124">Идентификатор строки отображаемого имени категории</span><span class="sxs-lookup"><span data-stu-id="f2fc5-124">The string id of the category's display name</span></span>|
|<span data-ttu-id="f2fc5-125">Корень</span><span class="sxs-lookup"><span data-stu-id="f2fc5-125">isRoot</span></span>|<span data-ttu-id="f2fc5-126">Логическое</span><span class="sxs-lookup"><span data-stu-id="f2fc5-126">Boolean</span></span>|<span data-ttu-id="f2fc5-127">Определяет, является ли категория корневой категорией</span><span class="sxs-lookup"><span data-stu-id="f2fc5-127">Defines if the category is a root category</span></span>|
|<span data-ttu-id="f2fc5-128">id</span><span class="sxs-lookup"><span data-stu-id="f2fc5-128">id</span></span>|<span data-ttu-id="f2fc5-129">String</span><span class="sxs-lookup"><span data-stu-id="f2fc5-129">String</span></span>|<span data-ttu-id="f2fc5-130">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f2fc5-130">Key of the entity.</span></span>|
|<span data-ttu-id="f2fc5-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fc5-131">lastModifiedDateTime</span></span>|<span data-ttu-id="f2fc5-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fc5-132">DateTimeOffset</span></span>|<span data-ttu-id="f2fc5-133">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f2fc5-133">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2fc5-134">Связи</span><span class="sxs-lookup"><span data-stu-id="f2fc5-134">Relationships</span></span>
|<span data-ttu-id="f2fc5-135">Связь</span><span class="sxs-lookup"><span data-stu-id="f2fc5-135">Relationship</span></span>|<span data-ttu-id="f2fc5-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f2fc5-136">Type</span></span>|<span data-ttu-id="f2fc5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f2fc5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fc5-138">верхнего</span><span class="sxs-lookup"><span data-stu-id="f2fc5-138">parent</span></span>|[<span data-ttu-id="f2fc5-139">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="f2fc5-139">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="f2fc5-140">Родительская категория</span><span class="sxs-lookup"><span data-stu-id="f2fc5-140">The parent category</span></span>|
|<span data-ttu-id="f2fc5-141">children</span><span class="sxs-lookup"><span data-stu-id="f2fc5-141">children</span></span>|<span data-ttu-id="f2fc5-142">Коллекция [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="f2fc5-142">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="f2fc5-143">Категории дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="f2fc5-143">The children categories</span></span>|
|<span data-ttu-id="f2fc5-144">определения</span><span class="sxs-lookup"><span data-stu-id="f2fc5-144">definitions</span></span>|<span data-ttu-id="f2fc5-145">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f2fc5-145">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="f2fc5-146">Непосредственный дочерний элемент Граупполицидефинитион в категории</span><span class="sxs-lookup"><span data-stu-id="f2fc5-146">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="f2fc5-147">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="f2fc5-147">definitionFile</span></span>|[<span data-ttu-id="f2fc5-148">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="f2fc5-148">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="f2fc5-149">Идентификатор файла определения, из которого получена Категория</span><span class="sxs-lookup"><span data-stu-id="f2fc5-149">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2fc5-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2fc5-150">JSON Representation</span></span>
<span data-ttu-id="f2fc5-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2fc5-151">Here is a JSON representation of the resource.</span></span>
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



