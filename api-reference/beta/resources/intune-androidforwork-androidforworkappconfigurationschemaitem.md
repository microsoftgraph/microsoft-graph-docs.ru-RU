---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 086da317eedc908ea44a7ec0d1b9140bbe0534b4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795193"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="c1db9-103">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="c1db9-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="c1db9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1db9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1db9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1db9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1db9-106">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="c1db9-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="c1db9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1db9-107">Properties</span></span>
|<span data-ttu-id="c1db9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1db9-108">Property</span></span>|<span data-ttu-id="c1db9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1db9-109">Type</span></span>|<span data-ttu-id="c1db9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1db9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1db9-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="c1db9-111">schemaItemKey</span></span>|<span data-ttu-id="c1db9-112">String</span><span class="sxs-lookup"><span data-stu-id="c1db9-112">String</span></span>|<span data-ttu-id="c1db9-113">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="c1db9-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="c1db9-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c1db9-114">displayName</span></span>|<span data-ttu-id="c1db9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c1db9-115">String</span></span>|<span data-ttu-id="c1db9-116">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="c1db9-116">Human readable name</span></span>|
|<span data-ttu-id="c1db9-117">description</span><span class="sxs-lookup"><span data-stu-id="c1db9-117">description</span></span>|<span data-ttu-id="c1db9-118">String</span><span class="sxs-lookup"><span data-stu-id="c1db9-118">String</span></span>|<span data-ttu-id="c1db9-119">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="c1db9-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="c1db9-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="c1db9-120">defaultBoolValue</span></span>|<span data-ttu-id="c1db9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1db9-121">Boolean</span></span>|<span data-ttu-id="c1db9-122">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1db9-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1db9-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="c1db9-123">defaultIntValue</span></span>|<span data-ttu-id="c1db9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db9-124">Int32</span></span>|<span data-ttu-id="c1db9-125">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1db9-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1db9-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="c1db9-126">defaultStringValue</span></span>|<span data-ttu-id="c1db9-127">String</span><span class="sxs-lookup"><span data-stu-id="c1db9-127">String</span></span>|<span data-ttu-id="c1db9-128">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1db9-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1db9-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="c1db9-129">defaultStringArrayValue</span></span>|<span data-ttu-id="c1db9-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c1db9-130">String collection</span></span>|<span data-ttu-id="c1db9-131">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1db9-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1db9-132">dataType</span><span class="sxs-lookup"><span data-stu-id="c1db9-132">dataType</span></span>|[<span data-ttu-id="c1db9-133">Андроидфорворкаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="c1db9-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="c1db9-134">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="c1db9-134">The type of value this item describes.</span></span> <span data-ttu-id="c1db9-135">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="c1db9-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="c1db9-136">selections</span><span class="sxs-lookup"><span data-stu-id="c1db9-136">selections</span></span>|<span data-ttu-id="c1db9-137">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c1db9-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1db9-138">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="c1db9-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1db9-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1db9-139">Relationships</span></span>
<span data-ttu-id="c1db9-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c1db9-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1db9-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1db9-141">JSON Representation</span></span>
<span data-ttu-id="c1db9-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1db9-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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





