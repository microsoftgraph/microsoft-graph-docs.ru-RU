---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99a77dccc7bec8e4d28944ac9d5e5af16a98b462
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019693"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="f3cc3-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="f3cc3-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="f3cc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3cc3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3cc3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3cc3-107">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="f3cc3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3cc3-108">Properties</span></span>
|<span data-ttu-id="f3cc3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3cc3-109">Property</span></span>|<span data-ttu-id="f3cc3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3cc3-110">Type</span></span>|<span data-ttu-id="f3cc3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3cc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cc3-112">index</span><span class="sxs-lookup"><span data-stu-id="f3cc3-112">index</span></span>|<span data-ttu-id="f3cc3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f3cc3-113">Int32</span></span>|<span data-ttu-id="f3cc3-114">Уникальный индекс, который приложение использует для поддержки вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="f3cc3-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="f3cc3-115">парентиндекс</span><span class="sxs-lookup"><span data-stu-id="f3cc3-115">parentIndex</span></span>|<span data-ttu-id="f3cc3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f3cc3-116">Int32</span></span>|<span data-ttu-id="f3cc3-117">Индекс элемента родительской схемы для отслеживания вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="f3cc3-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="f3cc3-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="f3cc3-118">schemaItemKey</span></span>|<span data-ttu-id="f3cc3-119">String</span><span class="sxs-lookup"><span data-stu-id="f3cc3-119">String</span></span>|<span data-ttu-id="f3cc3-120">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="f3cc3-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f3cc3-121">displayName</span></span>|<span data-ttu-id="f3cc3-122">String</span><span class="sxs-lookup"><span data-stu-id="f3cc3-122">String</span></span>|<span data-ttu-id="f3cc3-123">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-123">Human readable name</span></span>|
|<span data-ttu-id="f3cc3-124">description</span><span class="sxs-lookup"><span data-stu-id="f3cc3-124">description</span></span>|<span data-ttu-id="f3cc3-125">String</span><span class="sxs-lookup"><span data-stu-id="f3cc3-125">String</span></span>|<span data-ttu-id="f3cc3-126">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="f3cc3-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="f3cc3-127">defaultBoolValue</span></span>|<span data-ttu-id="f3cc3-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3cc3-128">Boolean</span></span>|<span data-ttu-id="f3cc3-129">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f3cc3-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="f3cc3-130">defaultIntValue</span></span>|<span data-ttu-id="f3cc3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f3cc3-131">Int32</span></span>|<span data-ttu-id="f3cc3-132">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f3cc3-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="f3cc3-133">defaultStringValue</span></span>|<span data-ttu-id="f3cc3-134">String</span><span class="sxs-lookup"><span data-stu-id="f3cc3-134">String</span></span>|<span data-ttu-id="f3cc3-135">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f3cc3-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="f3cc3-136">defaultStringArrayValue</span></span>|<span data-ttu-id="f3cc3-137">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f3cc3-137">String collection</span></span>|<span data-ttu-id="f3cc3-138">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f3cc3-139">dataType</span><span class="sxs-lookup"><span data-stu-id="f3cc3-139">dataType</span></span>|[<span data-ttu-id="f3cc3-140">андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="f3cc3-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="f3cc3-141">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-141">The type of value this item describes.</span></span> <span data-ttu-id="f3cc3-142">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="f3cc3-143">selections</span><span class="sxs-lookup"><span data-stu-id="f3cc3-143">selections</span></span>|<span data-ttu-id="f3cc3-144">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f3cc3-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f3cc3-145">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="f3cc3-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3cc3-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3cc3-146">Relationships</span></span>
<span data-ttu-id="f3cc3-147">Нет</span><span class="sxs-lookup"><span data-stu-id="f3cc3-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3cc3-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3cc3-148">JSON Representation</span></span>
<span data-ttu-id="f3cc3-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3cc3-149">Here is a JSON representation of the resource.</span></span>
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






