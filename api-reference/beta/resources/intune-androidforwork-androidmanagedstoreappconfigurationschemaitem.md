---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6db7a9958599cbc073fa17eef542559a65af2b8e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799334"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="5bc3d-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="5bc3d-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="5bc3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bc3d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bc3d-106">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="5bc3d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bc3d-107">Properties</span></span>
|<span data-ttu-id="5bc3d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bc3d-108">Property</span></span>|<span data-ttu-id="5bc3d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5bc3d-109">Type</span></span>|<span data-ttu-id="5bc3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc3d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc3d-111">index</span><span class="sxs-lookup"><span data-stu-id="5bc3d-111">index</span></span>|<span data-ttu-id="5bc3d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5bc3d-112">Int32</span></span>|<span data-ttu-id="5bc3d-113">Уникальный индекс, который приложение использует для поддержки вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="5bc3d-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="5bc3d-114">парентиндекс</span><span class="sxs-lookup"><span data-stu-id="5bc3d-114">parentIndex</span></span>|<span data-ttu-id="5bc3d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="5bc3d-115">Int32</span></span>|<span data-ttu-id="5bc3d-116">Индекс элемента родительской схемы для отслеживания вложенных элементов схемы</span><span class="sxs-lookup"><span data-stu-id="5bc3d-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="5bc3d-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="5bc3d-117">schemaItemKey</span></span>|<span data-ttu-id="5bc3d-118">String</span><span class="sxs-lookup"><span data-stu-id="5bc3d-118">String</span></span>|<span data-ttu-id="5bc3d-119">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="5bc3d-120">displayName</span><span class="sxs-lookup"><span data-stu-id="5bc3d-120">displayName</span></span>|<span data-ttu-id="5bc3d-121">Строка</span><span class="sxs-lookup"><span data-stu-id="5bc3d-121">String</span></span>|<span data-ttu-id="5bc3d-122">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-122">Human readable name</span></span>|
|<span data-ttu-id="5bc3d-123">description</span><span class="sxs-lookup"><span data-stu-id="5bc3d-123">description</span></span>|<span data-ttu-id="5bc3d-124">String</span><span class="sxs-lookup"><span data-stu-id="5bc3d-124">String</span></span>|<span data-ttu-id="5bc3d-125">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="5bc3d-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="5bc3d-126">defaultBoolValue</span></span>|<span data-ttu-id="5bc3d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bc3d-127">Boolean</span></span>|<span data-ttu-id="5bc3d-128">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5bc3d-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="5bc3d-129">defaultIntValue</span></span>|<span data-ttu-id="5bc3d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="5bc3d-130">Int32</span></span>|<span data-ttu-id="5bc3d-131">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5bc3d-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="5bc3d-132">defaultStringValue</span></span>|<span data-ttu-id="5bc3d-133">String</span><span class="sxs-lookup"><span data-stu-id="5bc3d-133">String</span></span>|<span data-ttu-id="5bc3d-134">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5bc3d-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="5bc3d-135">defaultStringArrayValue</span></span>|<span data-ttu-id="5bc3d-136">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5bc3d-136">String collection</span></span>|<span data-ttu-id="5bc3d-137">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5bc3d-138">dataType</span><span class="sxs-lookup"><span data-stu-id="5bc3d-138">dataType</span></span>|[<span data-ttu-id="5bc3d-139">андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="5bc3d-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="5bc3d-140">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-140">The type of value this item describes.</span></span> <span data-ttu-id="5bc3d-141">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="5bc3d-142">selections</span><span class="sxs-lookup"><span data-stu-id="5bc3d-142">selections</span></span>|<span data-ttu-id="5bc3d-143">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5bc3d-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5bc3d-144">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="5bc3d-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bc3d-145">Связи</span><span class="sxs-lookup"><span data-stu-id="5bc3d-145">Relationships</span></span>
<span data-ttu-id="5bc3d-146">Нет</span><span class="sxs-lookup"><span data-stu-id="5bc3d-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bc3d-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bc3d-147">JSON Representation</span></span>
<span data-ttu-id="5bc3d-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bc3d-148">Here is a JSON representation of the resource.</span></span>
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



