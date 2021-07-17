---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c0ca5e88d9d4ac7d7b63dea49f8ff4aace8cc348
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467461"
---
# <a name="schema-resource-type"></a><span data-ttu-id="d94ba-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="d94ba-103">schema resource type</span></span>

<span data-ttu-id="d94ba-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d94ba-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="d94ba-105">Схема [подключения](externalconnectors-externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d94ba-105">The [connection](externalconnectors-externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="d94ba-106">Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы.</span><span class="sxs-lookup"><span data-stu-id="d94ba-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="d94ba-107">Перед добавлением элементов в связь вы должны зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="d94ba-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="d94ba-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d94ba-108">Methods</span></span>
|<span data-ttu-id="d94ba-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d94ba-109">Method</span></span>|<span data-ttu-id="d94ba-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d94ba-110">Return type</span></span>|<span data-ttu-id="d94ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d94ba-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d94ba-112">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="d94ba-112">Create schema</span></span>](../api/externalconnectors-schema-create.md)|[<span data-ttu-id="d94ba-113">schema</span><span class="sxs-lookup"><span data-stu-id="d94ba-113">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="d94ba-114">Создайте новый [объект схемы.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="d94ba-114">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>|
|[<span data-ttu-id="d94ba-115">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="d94ba-115">Get schema</span></span>](../api/externalconnectors-schema-get.md)|[<span data-ttu-id="d94ba-116">schema</span><span class="sxs-lookup"><span data-stu-id="d94ba-116">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="d94ba-117">Ознакомьтесь с свойствами и отношениями объекта [схемы.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="d94ba-117">Read the properties and relationships of a [schema](../resources/externalconnectors-schema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d94ba-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d94ba-118">Properties</span></span>
|<span data-ttu-id="d94ba-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d94ba-119">Property</span></span>|<span data-ttu-id="d94ba-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d94ba-120">Type</span></span>|<span data-ttu-id="d94ba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d94ba-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d94ba-122">baseType</span><span class="sxs-lookup"><span data-stu-id="d94ba-122">baseType</span></span>|<span data-ttu-id="d94ba-123">String</span><span class="sxs-lookup"><span data-stu-id="d94ba-123">String</span></span>|<span data-ttu-id="d94ba-124">Необходимо указать значение `microsoft.graph.externalConnector.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="d94ba-124">Must be set to `microsoft.graph.externalConnector.externalItem`.</span></span> <span data-ttu-id="d94ba-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d94ba-125">Required.</span></span>|
|<span data-ttu-id="d94ba-126">properties</span><span class="sxs-lookup"><span data-stu-id="d94ba-126">properties</span></span>|<span data-ttu-id="d94ba-127">[коллекция](../resources/externalconnectors-property.md) свойств</span><span class="sxs-lookup"><span data-stu-id="d94ba-127">[property](../resources/externalconnectors-property.md) collection</span></span>|<span data-ttu-id="d94ba-128">Свойства, определенные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="d94ba-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="d94ba-129">Минимальное число свойств — одно, максимальное — 128.</span><span class="sxs-lookup"><span data-stu-id="d94ba-129">The minimum number of properties is one, the maximum is 128.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d94ba-130">Связи</span><span class="sxs-lookup"><span data-stu-id="d94ba-130">Relationships</span></span>
<span data-ttu-id="d94ba-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d94ba-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d94ba-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d94ba-132">JSON representation</span></span>
<span data-ttu-id="d94ba-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d94ba-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

