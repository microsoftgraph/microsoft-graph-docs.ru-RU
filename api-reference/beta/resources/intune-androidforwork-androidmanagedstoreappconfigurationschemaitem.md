---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2168cc2449092249ec07f17831c38b5be15d7676
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971692"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="04d41-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="04d41-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="04d41-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04d41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04d41-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04d41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04d41-106">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="04d41-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="04d41-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="04d41-107">Properties</span></span>
|<span data-ttu-id="04d41-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="04d41-108">Property</span></span>|<span data-ttu-id="04d41-109">Тип</span><span class="sxs-lookup"><span data-stu-id="04d41-109">Type</span></span>|<span data-ttu-id="04d41-110">Описание</span><span class="sxs-lookup"><span data-stu-id="04d41-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04d41-111">index</span><span class="sxs-lookup"><span data-stu-id="04d41-111">index</span></span>|<span data-ttu-id="04d41-112">Int32</span><span class="sxs-lookup"><span data-stu-id="04d41-112">Int32</span></span>|<span data-ttu-id="04d41-113">Уникальный индекс, который приложение использует для поддержки вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="04d41-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="04d41-114">Парентиндекс</span><span class="sxs-lookup"><span data-stu-id="04d41-114">parentIndex</span></span>|<span data-ttu-id="04d41-115">Int32</span><span class="sxs-lookup"><span data-stu-id="04d41-115">Int32</span></span>|<span data-ttu-id="04d41-116">Индекс элемента родительской схемы для отслеживания вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="04d41-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="04d41-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="04d41-117">schemaItemKey</span></span>|<span data-ttu-id="04d41-118">String</span><span class="sxs-lookup"><span data-stu-id="04d41-118">String</span></span>|<span data-ttu-id="04d41-119">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="04d41-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="04d41-120">displayName</span><span class="sxs-lookup"><span data-stu-id="04d41-120">displayName</span></span>|<span data-ttu-id="04d41-121">Строка</span><span class="sxs-lookup"><span data-stu-id="04d41-121">String</span></span>|<span data-ttu-id="04d41-122">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="04d41-122">Human readable name</span></span>|
|<span data-ttu-id="04d41-123">description</span><span class="sxs-lookup"><span data-stu-id="04d41-123">description</span></span>|<span data-ttu-id="04d41-124">String</span><span class="sxs-lookup"><span data-stu-id="04d41-124">String</span></span>|<span data-ttu-id="04d41-125">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="04d41-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="04d41-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="04d41-126">defaultBoolValue</span></span>|<span data-ttu-id="04d41-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="04d41-127">Boolean</span></span>|<span data-ttu-id="04d41-128">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="04d41-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="04d41-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="04d41-129">defaultIntValue</span></span>|<span data-ttu-id="04d41-130">Int32</span><span class="sxs-lookup"><span data-stu-id="04d41-130">Int32</span></span>|<span data-ttu-id="04d41-131">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="04d41-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="04d41-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="04d41-132">defaultStringValue</span></span>|<span data-ttu-id="04d41-133">String</span><span class="sxs-lookup"><span data-stu-id="04d41-133">String</span></span>|<span data-ttu-id="04d41-134">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="04d41-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="04d41-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="04d41-135">defaultStringArrayValue</span></span>|<span data-ttu-id="04d41-136">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="04d41-136">String collection</span></span>|<span data-ttu-id="04d41-137">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="04d41-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="04d41-138">dataType</span><span class="sxs-lookup"><span data-stu-id="04d41-138">dataType</span></span>|[<span data-ttu-id="04d41-139">Андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="04d41-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="04d41-140">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="04d41-140">The type of value this item describes.</span></span> <span data-ttu-id="04d41-141">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="04d41-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="04d41-142">selections</span><span class="sxs-lookup"><span data-stu-id="04d41-142">selections</span></span>|<span data-ttu-id="04d41-143">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="04d41-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="04d41-144">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="04d41-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="04d41-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="04d41-145">Relationships</span></span>
<span data-ttu-id="04d41-146">Нет</span><span class="sxs-lookup"><span data-stu-id="04d41-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04d41-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04d41-147">JSON Representation</span></span>
<span data-ttu-id="04d41-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04d41-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```





