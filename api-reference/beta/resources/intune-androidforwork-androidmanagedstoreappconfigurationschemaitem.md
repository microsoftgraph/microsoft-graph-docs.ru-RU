---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 706a4daa53201f8bdf295ca26ecf6f20134437da
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991417"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="55954-103">Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем</span><span class="sxs-lookup"><span data-stu-id="55954-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="55954-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55954-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55954-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55954-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55954-106">Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.</span><span class="sxs-lookup"><span data-stu-id="55954-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="55954-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55954-107">Properties</span></span>
|<span data-ttu-id="55954-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55954-108">Property</span></span>|<span data-ttu-id="55954-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55954-109">Type</span></span>|<span data-ttu-id="55954-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55954-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55954-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="55954-111">schemaItemKey</span></span>|<span data-ttu-id="55954-112">String</span><span class="sxs-lookup"><span data-stu-id="55954-112">String</span></span>|<span data-ttu-id="55954-113">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="55954-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="55954-114">displayName</span><span class="sxs-lookup"><span data-stu-id="55954-114">displayName</span></span>|<span data-ttu-id="55954-115">Строка</span><span class="sxs-lookup"><span data-stu-id="55954-115">String</span></span>|<span data-ttu-id="55954-116">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="55954-116">Human readable name</span></span>|
|<span data-ttu-id="55954-117">description</span><span class="sxs-lookup"><span data-stu-id="55954-117">description</span></span>|<span data-ttu-id="55954-118">String</span><span class="sxs-lookup"><span data-stu-id="55954-118">String</span></span>|<span data-ttu-id="55954-119">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="55954-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="55954-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="55954-120">defaultBoolValue</span></span>|<span data-ttu-id="55954-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="55954-121">Boolean</span></span>|<span data-ttu-id="55954-122">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="55954-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="55954-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="55954-123">defaultIntValue</span></span>|<span data-ttu-id="55954-124">Int32</span><span class="sxs-lookup"><span data-stu-id="55954-124">Int32</span></span>|<span data-ttu-id="55954-125">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="55954-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="55954-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="55954-126">defaultStringValue</span></span>|<span data-ttu-id="55954-127">String</span><span class="sxs-lookup"><span data-stu-id="55954-127">String</span></span>|<span data-ttu-id="55954-128">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="55954-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="55954-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="55954-129">defaultStringArrayValue</span></span>|<span data-ttu-id="55954-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="55954-130">String collection</span></span>|<span data-ttu-id="55954-131">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="55954-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="55954-132">dataType</span><span class="sxs-lookup"><span data-stu-id="55954-132">dataType</span></span>|[<span data-ttu-id="55954-133">Андроидманажедстореаппконфигуратионсчемаитемдататипе</span><span class="sxs-lookup"><span data-stu-id="55954-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="55954-134">Тип значения, который описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="55954-134">The type of value this item describes.</span></span> <span data-ttu-id="55954-135">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="55954-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="55954-136">selections</span><span class="sxs-lookup"><span data-stu-id="55954-136">selections</span></span>|<span data-ttu-id="55954-137">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="55954-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="55954-138">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="55954-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="55954-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="55954-139">Relationships</span></span>
<span data-ttu-id="55954-140">Нет</span><span class="sxs-lookup"><span data-stu-id="55954-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55954-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55954-141">JSON Representation</span></span>
<span data-ttu-id="55954-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55954-142">Here is a JSON representation of the resource.</span></span>
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





