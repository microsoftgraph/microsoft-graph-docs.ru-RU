---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60bfa322af19a71dc02213a64aa5d9f067f5c3c7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702665"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="f29c4-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="f29c4-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="f29c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f29c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f29c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f29c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f29c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f29c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f29c4-107">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="f29c4-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="f29c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f29c4-108">Properties</span></span>
|<span data-ttu-id="f29c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f29c4-109">Property</span></span>|<span data-ttu-id="f29c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f29c4-110">Type</span></span>|<span data-ttu-id="f29c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f29c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29c4-112">index</span><span class="sxs-lookup"><span data-stu-id="f29c4-112">index</span></span>|<span data-ttu-id="f29c4-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f29c4-113">Int32</span></span>|<span data-ttu-id="f29c4-114">Уникальный индекс, который приложение использует для поддержки вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="f29c4-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="f29c4-115">парентиндекс</span><span class="sxs-lookup"><span data-stu-id="f29c4-115">parentIndex</span></span>|<span data-ttu-id="f29c4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f29c4-116">Int32</span></span>|<span data-ttu-id="f29c4-117">Индекс элемента родительской схемы для отслеживания вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="f29c4-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="f29c4-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="f29c4-118">schemaItemKey</span></span>|<span data-ttu-id="f29c4-119">String</span><span class="sxs-lookup"><span data-stu-id="f29c4-119">String</span></span>|<span data-ttu-id="f29c4-120">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="f29c4-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="f29c4-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f29c4-121">displayName</span></span>|<span data-ttu-id="f29c4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="f29c4-122">String</span></span>|<span data-ttu-id="f29c4-123">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="f29c4-123">Human readable name</span></span>|
|<span data-ttu-id="f29c4-124">description</span><span class="sxs-lookup"><span data-stu-id="f29c4-124">description</span></span>|<span data-ttu-id="f29c4-125">Строка</span><span class="sxs-lookup"><span data-stu-id="f29c4-125">String</span></span>|<span data-ttu-id="f29c4-126">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="f29c4-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="f29c4-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="f29c4-127">defaultBoolValue</span></span>|<span data-ttu-id="f29c4-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f29c4-128">Boolean</span></span>|<span data-ttu-id="f29c4-129">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f29c4-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f29c4-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="f29c4-130">defaultIntValue</span></span>|<span data-ttu-id="f29c4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f29c4-131">Int32</span></span>|<span data-ttu-id="f29c4-132">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f29c4-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f29c4-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="f29c4-133">defaultStringValue</span></span>|<span data-ttu-id="f29c4-134">String</span><span class="sxs-lookup"><span data-stu-id="f29c4-134">String</span></span>|<span data-ttu-id="f29c4-135">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f29c4-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f29c4-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="f29c4-136">defaultStringArrayValue</span></span>|<span data-ttu-id="f29c4-137">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f29c4-137">String collection</span></span>|<span data-ttu-id="f29c4-138">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="f29c4-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f29c4-139">dataType</span><span class="sxs-lookup"><span data-stu-id="f29c4-139">dataType</span></span>|[<span data-ttu-id="f29c4-140">андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="f29c4-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="f29c4-141">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="f29c4-141">The type of value this item describes.</span></span> <span data-ttu-id="f29c4-142">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="f29c4-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="f29c4-143">selections</span><span class="sxs-lookup"><span data-stu-id="f29c4-143">selections</span></span>|<span data-ttu-id="f29c4-144">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f29c4-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f29c4-145">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="f29c4-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f29c4-146">Связи</span><span class="sxs-lookup"><span data-stu-id="f29c4-146">Relationships</span></span>
<span data-ttu-id="f29c4-147">Нет</span><span class="sxs-lookup"><span data-stu-id="f29c4-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f29c4-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f29c4-148">JSON Representation</span></span>
<span data-ttu-id="f29c4-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f29c4-149">Here is a JSON representation of the resource.</span></span>
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





