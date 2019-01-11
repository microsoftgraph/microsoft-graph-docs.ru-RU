---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
localization_priority: Normal
ms.openlocfilehash: 1fb6cb56f754b6d2b100ea2f4d666e31c21efaaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890897"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="a2c60-103">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="a2c60-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="a2c60-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2c60-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2c60-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2c60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2c60-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2c60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2c60-107">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="a2c60-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="a2c60-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2c60-108">Properties</span></span>
|<span data-ttu-id="a2c60-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2c60-109">Property</span></span>|<span data-ttu-id="a2c60-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a2c60-110">Type</span></span>|<span data-ttu-id="a2c60-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a2c60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2c60-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="a2c60-112">schemaItemKey</span></span>|<span data-ttu-id="a2c60-113">String</span><span class="sxs-lookup"><span data-stu-id="a2c60-113">String</span></span>|<span data-ttu-id="a2c60-114">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="a2c60-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="a2c60-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a2c60-115">displayName</span></span>|<span data-ttu-id="a2c60-116">String</span><span class="sxs-lookup"><span data-stu-id="a2c60-116">String</span></span>|<span data-ttu-id="a2c60-117">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="a2c60-117">Human readable name</span></span>|
|<span data-ttu-id="a2c60-118">описание</span><span class="sxs-lookup"><span data-stu-id="a2c60-118">description</span></span>|<span data-ttu-id="a2c60-119">String</span><span class="sxs-lookup"><span data-stu-id="a2c60-119">String</span></span>|<span data-ttu-id="a2c60-120">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="a2c60-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="a2c60-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="a2c60-121">defaultBoolValue</span></span>|<span data-ttu-id="a2c60-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2c60-122">Boolean</span></span>|<span data-ttu-id="a2c60-123">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="a2c60-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a2c60-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="a2c60-124">defaultIntValue</span></span>|<span data-ttu-id="a2c60-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a2c60-125">Int32</span></span>|<span data-ttu-id="a2c60-126">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="a2c60-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a2c60-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="a2c60-127">defaultStringValue</span></span>|<span data-ttu-id="a2c60-128">String</span><span class="sxs-lookup"><span data-stu-id="a2c60-128">String</span></span>|<span data-ttu-id="a2c60-129">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="a2c60-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a2c60-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="a2c60-130">defaultStringArrayValue</span></span>|<span data-ttu-id="a2c60-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2c60-131">String collection</span></span>|<span data-ttu-id="a2c60-132">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="a2c60-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a2c60-133">dataType</span><span class="sxs-lookup"><span data-stu-id="a2c60-133">dataType</span></span>|[<span data-ttu-id="a2c60-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="a2c60-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="a2c60-135">Введите значение, которое описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="a2c60-135">The type of value this item describes.</span></span> <span data-ttu-id="a2c60-136">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="a2c60-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="a2c60-137">selections</span><span class="sxs-lookup"><span data-stu-id="a2c60-137">selections</span></span>|<span data-ttu-id="a2c60-138">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a2c60-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a2c60-139">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="a2c60-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2c60-140">Связи</span><span class="sxs-lookup"><span data-stu-id="a2c60-140">Relationships</span></span>
<span data-ttu-id="a2c60-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a2c60-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2c60-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2c60-142">JSON Representation</span></span>
<span data-ttu-id="a2c60-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2c60-143">Here is a JSON representation of the resource.</span></span>
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





