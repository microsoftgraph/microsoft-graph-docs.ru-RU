---
title: Тип ресурса androidManagedStoreAppConfigurationSchemaItem
description: Конфигурация отдельного элемента внутри схемы настраиваемой конфигурации Android приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398921"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="6664a-103">Тип ресурса androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="6664a-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="6664a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6664a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6664a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6664a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6664a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6664a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6664a-107">Конфигурация отдельного элемента внутри схемы настраиваемой конфигурации Android приложения.</span><span class="sxs-lookup"><span data-stu-id="6664a-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="6664a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6664a-108">Properties</span></span>
|<span data-ttu-id="6664a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6664a-109">Property</span></span>|<span data-ttu-id="6664a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6664a-110">Type</span></span>|<span data-ttu-id="6664a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6664a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6664a-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="6664a-112">schemaItemKey</span></span>|<span data-ttu-id="6664a-113">String</span><span class="sxs-lookup"><span data-stu-id="6664a-113">String</span></span>|<span data-ttu-id="6664a-114">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="6664a-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="6664a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6664a-115">displayName</span></span>|<span data-ttu-id="6664a-116">String</span><span class="sxs-lookup"><span data-stu-id="6664a-116">String</span></span>|<span data-ttu-id="6664a-117">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="6664a-117">Human readable name</span></span>|
|<span data-ttu-id="6664a-118">description</span><span class="sxs-lookup"><span data-stu-id="6664a-118">description</span></span>|<span data-ttu-id="6664a-119">String</span><span class="sxs-lookup"><span data-stu-id="6664a-119">String</span></span>|<span data-ttu-id="6664a-120">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="6664a-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="6664a-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="6664a-121">defaultBoolValue</span></span>|<span data-ttu-id="6664a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6664a-122">Boolean</span></span>|<span data-ttu-id="6664a-123">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6664a-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6664a-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="6664a-124">defaultIntValue</span></span>|<span data-ttu-id="6664a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6664a-125">Int32</span></span>|<span data-ttu-id="6664a-126">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6664a-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6664a-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="6664a-127">defaultStringValue</span></span>|<span data-ttu-id="6664a-128">String</span><span class="sxs-lookup"><span data-stu-id="6664a-128">String</span></span>|<span data-ttu-id="6664a-129">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6664a-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6664a-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="6664a-130">defaultStringArrayValue</span></span>|<span data-ttu-id="6664a-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="6664a-131">String collection</span></span>|<span data-ttu-id="6664a-132">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6664a-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6664a-133">dataType</span><span class="sxs-lookup"><span data-stu-id="6664a-133">dataType</span></span>|[<span data-ttu-id="6664a-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="6664a-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="6664a-135">Введите значение, которое описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="6664a-135">The type of value this item describes.</span></span> <span data-ttu-id="6664a-136">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="6664a-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="6664a-137">selections</span><span class="sxs-lookup"><span data-stu-id="6664a-137">selections</span></span>|<span data-ttu-id="6664a-138">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6664a-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6664a-139">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="6664a-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6664a-140">Связи</span><span class="sxs-lookup"><span data-stu-id="6664a-140">Relationships</span></span>
<span data-ttu-id="6664a-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6664a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6664a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6664a-142">JSON Representation</span></span>
<span data-ttu-id="6664a-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6664a-143">Here is a JSON representation of the resource.</span></span>
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




