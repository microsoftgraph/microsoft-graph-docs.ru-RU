---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0de75506419ea0e403c7f55af07459514abb408c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147735"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="c1d38-103">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="c1d38-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="c1d38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1d38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1d38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1d38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1d38-106">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="c1d38-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="c1d38-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1d38-107">Properties</span></span>
|<span data-ttu-id="c1d38-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1d38-108">Property</span></span>|<span data-ttu-id="c1d38-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1d38-109">Type</span></span>|<span data-ttu-id="c1d38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1d38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d38-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="c1d38-111">schemaItemKey</span></span>|<span data-ttu-id="c1d38-112">String</span><span class="sxs-lookup"><span data-stu-id="c1d38-112">String</span></span>|<span data-ttu-id="c1d38-113">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="c1d38-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="c1d38-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c1d38-114">displayName</span></span>|<span data-ttu-id="c1d38-115">String</span><span class="sxs-lookup"><span data-stu-id="c1d38-115">String</span></span>|<span data-ttu-id="c1d38-116">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="c1d38-116">Human readable name</span></span>|
|<span data-ttu-id="c1d38-117">description</span><span class="sxs-lookup"><span data-stu-id="c1d38-117">description</span></span>|<span data-ttu-id="c1d38-118">String</span><span class="sxs-lookup"><span data-stu-id="c1d38-118">String</span></span>|<span data-ttu-id="c1d38-119">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="c1d38-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="c1d38-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="c1d38-120">defaultBoolValue</span></span>|<span data-ttu-id="c1d38-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1d38-121">Boolean</span></span>|<span data-ttu-id="c1d38-122">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1d38-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1d38-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="c1d38-123">defaultIntValue</span></span>|<span data-ttu-id="c1d38-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c1d38-124">Int32</span></span>|<span data-ttu-id="c1d38-125">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1d38-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1d38-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="c1d38-126">defaultStringValue</span></span>|<span data-ttu-id="c1d38-127">String</span><span class="sxs-lookup"><span data-stu-id="c1d38-127">String</span></span>|<span data-ttu-id="c1d38-128">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1d38-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1d38-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="c1d38-129">defaultStringArrayValue</span></span>|<span data-ttu-id="c1d38-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c1d38-130">String collection</span></span>|<span data-ttu-id="c1d38-131">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="c1d38-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c1d38-132">dataType</span><span class="sxs-lookup"><span data-stu-id="c1d38-132">dataType</span></span>|[<span data-ttu-id="c1d38-133">Андроидфорворкаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="c1d38-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="c1d38-134">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="c1d38-134">The type of value this item describes.</span></span> <span data-ttu-id="c1d38-135">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="c1d38-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="c1d38-136">selections</span><span class="sxs-lookup"><span data-stu-id="c1d38-136">selections</span></span>|<span data-ttu-id="c1d38-137">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c1d38-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1d38-138">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="c1d38-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1d38-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c1d38-139">Relationships</span></span>
<span data-ttu-id="c1d38-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c1d38-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1d38-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1d38-141">JSON Representation</span></span>
<span data-ttu-id="c1d38-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1d38-142">Here is a JSON representation of the resource.</span></span>
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




