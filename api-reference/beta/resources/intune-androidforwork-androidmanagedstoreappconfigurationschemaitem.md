---
title: Тип ресурса androidManagedStoreAppConfigurationSchemaItem
description: Конфигурация отдельного элемента внутри схемы настраиваемой конфигурации Android приложения.
ms.openlocfilehash: 94ae8735800e4f79be2e7c61f8b971bafd8c394f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080897"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="6f51e-103">Тип ресурса androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="6f51e-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="6f51e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f51e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f51e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f51e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f51e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f51e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f51e-107">Конфигурация отдельного элемента внутри схемы настраиваемой конфигурации Android приложения.</span><span class="sxs-lookup"><span data-stu-id="6f51e-107">Single configuration item inside an Android application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="6f51e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f51e-108">Properties</span></span>
|<span data-ttu-id="6f51e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f51e-109">Property</span></span>|<span data-ttu-id="6f51e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6f51e-110">Type</span></span>|<span data-ttu-id="6f51e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f51e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f51e-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="6f51e-112">schemaItemKey</span></span>|<span data-ttu-id="6f51e-113">String</span><span class="sxs-lookup"><span data-stu-id="6f51e-113">String</span></span>|<span data-ttu-id="6f51e-114">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="6f51e-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="6f51e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6f51e-115">displayName</span></span>|<span data-ttu-id="6f51e-116">String</span><span class="sxs-lookup"><span data-stu-id="6f51e-116">String</span></span>|<span data-ttu-id="6f51e-117">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="6f51e-117">Human readable name</span></span>|
|<span data-ttu-id="6f51e-118">описание</span><span class="sxs-lookup"><span data-stu-id="6f51e-118">description</span></span>|<span data-ttu-id="6f51e-119">String</span><span class="sxs-lookup"><span data-stu-id="6f51e-119">String</span></span>|<span data-ttu-id="6f51e-120">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="6f51e-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="6f51e-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="6f51e-121">defaultBoolValue</span></span>|<span data-ttu-id="6f51e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f51e-122">Boolean</span></span>|<span data-ttu-id="6f51e-123">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6f51e-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6f51e-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="6f51e-124">defaultIntValue</span></span>|<span data-ttu-id="6f51e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6f51e-125">Int32</span></span>|<span data-ttu-id="6f51e-126">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6f51e-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6f51e-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="6f51e-127">defaultStringValue</span></span>|<span data-ttu-id="6f51e-128">String</span><span class="sxs-lookup"><span data-stu-id="6f51e-128">String</span></span>|<span data-ttu-id="6f51e-129">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6f51e-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6f51e-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="6f51e-130">defaultStringArrayValue</span></span>|<span data-ttu-id="6f51e-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="6f51e-131">String collection</span></span>|<span data-ttu-id="6f51e-132">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6f51e-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6f51e-133">dataType</span><span class="sxs-lookup"><span data-stu-id="6f51e-133">dataType</span></span>|[<span data-ttu-id="6f51e-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="6f51e-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="6f51e-135">Введите значение, которое описывает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="6f51e-135">The type of value this item describes.</span></span> <span data-ttu-id="6f51e-136">Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="6f51e-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="6f51e-137">selections</span><span class="sxs-lookup"><span data-stu-id="6f51e-137">selections</span></span>|<span data-ttu-id="6f51e-138">Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6f51e-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6f51e-139">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="6f51e-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f51e-140">Связи</span><span class="sxs-lookup"><span data-stu-id="6f51e-140">Relationships</span></span>
<span data-ttu-id="6f51e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6f51e-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f51e-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f51e-142">JSON Representation</span></span>
<span data-ttu-id="6f51e-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f51e-143">Here is a JSON representation of the resource.</span></span>
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





