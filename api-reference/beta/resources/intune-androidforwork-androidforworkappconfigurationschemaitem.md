---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13af3b581498a4285773b2fda02d5596127c3012
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019672"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="9bb84-103">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="9bb84-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="9bb84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bb84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bb84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bb84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bb84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bb84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb84-107">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="9bb84-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="9bb84-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bb84-108">Properties</span></span>
|<span data-ttu-id="9bb84-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bb84-109">Property</span></span>|<span data-ttu-id="9bb84-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bb84-110">Type</span></span>|<span data-ttu-id="9bb84-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bb84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb84-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="9bb84-112">schemaItemKey</span></span>|<span data-ttu-id="9bb84-113">String</span><span class="sxs-lookup"><span data-stu-id="9bb84-113">String</span></span>|<span data-ttu-id="9bb84-114">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="9bb84-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="9bb84-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9bb84-115">displayName</span></span>|<span data-ttu-id="9bb84-116">String</span><span class="sxs-lookup"><span data-stu-id="9bb84-116">String</span></span>|<span data-ttu-id="9bb84-117">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="9bb84-117">Human readable name</span></span>|
|<span data-ttu-id="9bb84-118">description</span><span class="sxs-lookup"><span data-stu-id="9bb84-118">description</span></span>|<span data-ttu-id="9bb84-119">String</span><span class="sxs-lookup"><span data-stu-id="9bb84-119">String</span></span>|<span data-ttu-id="9bb84-120">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="9bb84-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="9bb84-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="9bb84-121">defaultBoolValue</span></span>|<span data-ttu-id="9bb84-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bb84-122">Boolean</span></span>|<span data-ttu-id="9bb84-123">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="9bb84-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9bb84-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="9bb84-124">defaultIntValue</span></span>|<span data-ttu-id="9bb84-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9bb84-125">Int32</span></span>|<span data-ttu-id="9bb84-126">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="9bb84-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9bb84-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="9bb84-127">defaultStringValue</span></span>|<span data-ttu-id="9bb84-128">String</span><span class="sxs-lookup"><span data-stu-id="9bb84-128">String</span></span>|<span data-ttu-id="9bb84-129">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="9bb84-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9bb84-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="9bb84-130">defaultStringArrayValue</span></span>|<span data-ttu-id="9bb84-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="9bb84-131">String collection</span></span>|<span data-ttu-id="9bb84-132">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="9bb84-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9bb84-133">dataType</span><span class="sxs-lookup"><span data-stu-id="9bb84-133">dataType</span></span>|[<span data-ttu-id="9bb84-134">андроидфорворкаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="9bb84-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="9bb84-135">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="9bb84-135">The type of value this item describes.</span></span> <span data-ttu-id="9bb84-136">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="9bb84-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="9bb84-137">selections</span><span class="sxs-lookup"><span data-stu-id="9bb84-137">selections</span></span>|<span data-ttu-id="9bb84-138">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9bb84-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9bb84-139">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="9bb84-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bb84-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="9bb84-140">Relationships</span></span>
<span data-ttu-id="9bb84-141">Нет</span><span class="sxs-lookup"><span data-stu-id="9bb84-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bb84-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bb84-142">JSON Representation</span></span>
<span data-ttu-id="9bb84-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bb84-143">Here is a JSON representation of the resource.</span></span>
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






