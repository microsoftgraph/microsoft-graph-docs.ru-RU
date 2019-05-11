---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3012542315cd30a565da315a9d383757557b1008
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950545"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="5a67c-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="5a67c-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="5a67c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a67c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a67c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a67c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a67c-106">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="5a67c-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="5a67c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a67c-107">Properties</span></span>
|<span data-ttu-id="5a67c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a67c-108">Property</span></span>|<span data-ttu-id="5a67c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a67c-109">Type</span></span>|<span data-ttu-id="5a67c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a67c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a67c-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="5a67c-111">schemaItemKey</span></span>|<span data-ttu-id="5a67c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5a67c-112">String</span></span>|<span data-ttu-id="5a67c-113">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="5a67c-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="5a67c-114">displayName</span><span class="sxs-lookup"><span data-stu-id="5a67c-114">displayName</span></span>|<span data-ttu-id="5a67c-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5a67c-115">String</span></span>|<span data-ttu-id="5a67c-116">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="5a67c-116">Human readable name</span></span>|
|<span data-ttu-id="5a67c-117">description</span><span class="sxs-lookup"><span data-stu-id="5a67c-117">description</span></span>|<span data-ttu-id="5a67c-118">String</span><span class="sxs-lookup"><span data-stu-id="5a67c-118">String</span></span>|<span data-ttu-id="5a67c-119">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="5a67c-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="5a67c-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="5a67c-120">defaultBoolValue</span></span>|<span data-ttu-id="5a67c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a67c-121">Boolean</span></span>|<span data-ttu-id="5a67c-122">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5a67c-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5a67c-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="5a67c-123">defaultIntValue</span></span>|<span data-ttu-id="5a67c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5a67c-124">Int32</span></span>|<span data-ttu-id="5a67c-125">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5a67c-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5a67c-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="5a67c-126">defaultStringValue</span></span>|<span data-ttu-id="5a67c-127">String</span><span class="sxs-lookup"><span data-stu-id="5a67c-127">String</span></span>|<span data-ttu-id="5a67c-128">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5a67c-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5a67c-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="5a67c-129">defaultStringArrayValue</span></span>|<span data-ttu-id="5a67c-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5a67c-130">String collection</span></span>|<span data-ttu-id="5a67c-131">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5a67c-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5a67c-132">dataType</span><span class="sxs-lookup"><span data-stu-id="5a67c-132">dataType</span></span>|[<span data-ttu-id="5a67c-133">Андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="5a67c-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="5a67c-134">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="5a67c-134">The type of value this item describes.</span></span> <span data-ttu-id="5a67c-135">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="5a67c-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="5a67c-136">selections</span><span class="sxs-lookup"><span data-stu-id="5a67c-136">selections</span></span>|<span data-ttu-id="5a67c-137">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5a67c-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5a67c-138">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="5a67c-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a67c-139">Связи</span><span class="sxs-lookup"><span data-stu-id="5a67c-139">Relationships</span></span>
<span data-ttu-id="5a67c-140">Нет</span><span class="sxs-lookup"><span data-stu-id="5a67c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a67c-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a67c-141">JSON Representation</span></span>
<span data-ttu-id="5a67c-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a67c-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




