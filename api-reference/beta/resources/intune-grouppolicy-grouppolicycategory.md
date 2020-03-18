---
title: Тип ресурса Граупполицикатегори
description: Сущность Category сохраняет категорию определения групповой политики
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b754020cc4a7c4f7e9fdf7cc35f74d9dcc4c4c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783125"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="0cde8-103">Тип ресурса Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-103">groupPolicyCategory resource type</span></span>

> <span data-ttu-id="0cde8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cde8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cde8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cde8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cde8-106">Сущность Category сохраняет категорию определения групповой политики</span><span class="sxs-lookup"><span data-stu-id="0cde8-106">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="0cde8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0cde8-107">Methods</span></span>
|<span data-ttu-id="0cde8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0cde8-108">Method</span></span>|<span data-ttu-id="0cde8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cde8-109">Return Type</span></span>|<span data-ttu-id="0cde8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0cde8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cde8-111">Получение Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-111">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="0cde8-112">граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-112">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="0cde8-113">Чтение свойств и связей объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0cde8-113">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="0cde8-114">Обновление Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-114">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="0cde8-115">граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-115">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="0cde8-116">Обновление свойств объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0cde8-116">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cde8-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cde8-117">Properties</span></span>
|<span data-ttu-id="0cde8-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cde8-118">Property</span></span>|<span data-ttu-id="0cde8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0cde8-119">Type</span></span>|<span data-ttu-id="0cde8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0cde8-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cde8-121">displayName</span><span class="sxs-lookup"><span data-stu-id="0cde8-121">displayName</span></span>|<span data-ttu-id="0cde8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="0cde8-122">String</span></span>|<span data-ttu-id="0cde8-123">Идентификатор строки отображаемого имени категории</span><span class="sxs-lookup"><span data-stu-id="0cde8-123">The string id of the category's display name</span></span>|
|<span data-ttu-id="0cde8-124">Корень</span><span class="sxs-lookup"><span data-stu-id="0cde8-124">isRoot</span></span>|<span data-ttu-id="0cde8-125">Логический</span><span class="sxs-lookup"><span data-stu-id="0cde8-125">Boolean</span></span>|<span data-ttu-id="0cde8-126">Определяет, является ли категория корневой категорией</span><span class="sxs-lookup"><span data-stu-id="0cde8-126">Defines if the category is a root category</span></span>|
|<span data-ttu-id="0cde8-127">id</span><span class="sxs-lookup"><span data-stu-id="0cde8-127">id</span></span>|<span data-ttu-id="0cde8-128">String</span><span class="sxs-lookup"><span data-stu-id="0cde8-128">String</span></span>|<span data-ttu-id="0cde8-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0cde8-129">Key of the entity.</span></span>|
|<span data-ttu-id="0cde8-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cde8-130">lastModifiedDateTime</span></span>|<span data-ttu-id="0cde8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cde8-131">DateTimeOffset</span></span>|<span data-ttu-id="0cde8-132">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0cde8-132">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cde8-133">Связи</span><span class="sxs-lookup"><span data-stu-id="0cde8-133">Relationships</span></span>
|<span data-ttu-id="0cde8-134">Связь</span><span class="sxs-lookup"><span data-stu-id="0cde8-134">Relationship</span></span>|<span data-ttu-id="0cde8-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0cde8-135">Type</span></span>|<span data-ttu-id="0cde8-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0cde8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cde8-137">верхнего</span><span class="sxs-lookup"><span data-stu-id="0cde8-137">parent</span></span>|[<span data-ttu-id="0cde8-138">граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="0cde8-138">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="0cde8-139">Родительская категория</span><span class="sxs-lookup"><span data-stu-id="0cde8-139">The parent category</span></span>|
|<span data-ttu-id="0cde8-140">children</span><span class="sxs-lookup"><span data-stu-id="0cde8-140">children</span></span>|<span data-ttu-id="0cde8-141">Коллекция [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="0cde8-141">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="0cde8-142">Категории дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="0cde8-142">The children categories</span></span>|
|<span data-ttu-id="0cde8-143">определения</span><span class="sxs-lookup"><span data-stu-id="0cde8-143">definitions</span></span>|<span data-ttu-id="0cde8-144">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cde8-144">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="0cde8-145">Непосредственный дочерний элемент Граупполицидефинитион в категории</span><span class="sxs-lookup"><span data-stu-id="0cde8-145">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="0cde8-146">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="0cde8-146">definitionFile</span></span>|[<span data-ttu-id="0cde8-147">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="0cde8-147">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="0cde8-148">Идентификатор файла определения, из которого получена Категория</span><span class="sxs-lookup"><span data-stu-id="0cde8-148">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cde8-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cde8-149">JSON Representation</span></span>
<span data-ttu-id="0cde8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cde8-150">Here is a JSON representation of the resource.</span></span>
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



