---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e64edefe6da8b0c09b0eb90a6c772f34d908cf5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799419"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="15a17-103">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="15a17-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="15a17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15a17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15a17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15a17-106">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="15a17-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="15a17-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15a17-107">Properties</span></span>
|<span data-ttu-id="15a17-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15a17-108">Property</span></span>|<span data-ttu-id="15a17-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15a17-109">Type</span></span>|<span data-ttu-id="15a17-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15a17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15a17-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="15a17-111">schemaItemKey</span></span>|<span data-ttu-id="15a17-112">String</span><span class="sxs-lookup"><span data-stu-id="15a17-112">String</span></span>|<span data-ttu-id="15a17-113">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="15a17-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="15a17-114">displayName</span><span class="sxs-lookup"><span data-stu-id="15a17-114">displayName</span></span>|<span data-ttu-id="15a17-115">Строка</span><span class="sxs-lookup"><span data-stu-id="15a17-115">String</span></span>|<span data-ttu-id="15a17-116">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="15a17-116">Human readable name</span></span>|
|<span data-ttu-id="15a17-117">description</span><span class="sxs-lookup"><span data-stu-id="15a17-117">description</span></span>|<span data-ttu-id="15a17-118">String</span><span class="sxs-lookup"><span data-stu-id="15a17-118">String</span></span>|<span data-ttu-id="15a17-119">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="15a17-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="15a17-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="15a17-120">defaultBoolValue</span></span>|<span data-ttu-id="15a17-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="15a17-121">Boolean</span></span>|<span data-ttu-id="15a17-122">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="15a17-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="15a17-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="15a17-123">defaultIntValue</span></span>|<span data-ttu-id="15a17-124">Int32</span><span class="sxs-lookup"><span data-stu-id="15a17-124">Int32</span></span>|<span data-ttu-id="15a17-125">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="15a17-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="15a17-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="15a17-126">defaultStringValue</span></span>|<span data-ttu-id="15a17-127">String</span><span class="sxs-lookup"><span data-stu-id="15a17-127">String</span></span>|<span data-ttu-id="15a17-128">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="15a17-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="15a17-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="15a17-129">defaultStringArrayValue</span></span>|<span data-ttu-id="15a17-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="15a17-130">String collection</span></span>|<span data-ttu-id="15a17-131">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="15a17-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="15a17-132">dataType</span><span class="sxs-lookup"><span data-stu-id="15a17-132">dataType</span></span>|[<span data-ttu-id="15a17-133">андроидфорворкаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="15a17-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="15a17-134">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="15a17-134">The type of value this item describes.</span></span> <span data-ttu-id="15a17-135">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="15a17-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="15a17-136">selections</span><span class="sxs-lookup"><span data-stu-id="15a17-136">selections</span></span>|<span data-ttu-id="15a17-137">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="15a17-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="15a17-138">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="15a17-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="15a17-139">Связи</span><span class="sxs-lookup"><span data-stu-id="15a17-139">Relationships</span></span>
<span data-ttu-id="15a17-140">Нет</span><span class="sxs-lookup"><span data-stu-id="15a17-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15a17-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15a17-141">JSON Representation</span></span>
<span data-ttu-id="15a17-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15a17-142">Here is a JSON representation of the resource.</span></span>
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



