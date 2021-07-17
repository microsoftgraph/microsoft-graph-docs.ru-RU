---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 649f9e0ae8e0162e9fa4f976d5158e23bfb49b05
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467848"
---
# <a name="schema-resource-type"></a><span data-ttu-id="d4507-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="d4507-103">schema resource type</span></span>

<span data-ttu-id="d4507-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d4507-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4507-105">Схема [подключения](externalconnectors-externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4507-105">The [connection](externalconnectors-externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="d4507-106">Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы.</span><span class="sxs-lookup"><span data-stu-id="d4507-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="d4507-107">Перед добавлением элементов в связь вы должны зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="d4507-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="d4507-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d4507-108">Methods</span></span>

| <span data-ttu-id="d4507-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d4507-109">Method</span></span>                                                    | <span data-ttu-id="d4507-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4507-110">Return Type</span></span>                   | <span data-ttu-id="d4507-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4507-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="d4507-112">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="d4507-112">Create schema</span></span>](../api/externalconnectors-externalconnection-post-schema.md) | <span data-ttu-id="d4507-113">Нет *или* [схемы](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="d4507-113">None *or* [schema](externalconnectors-schema.md)</span></span> | <span data-ttu-id="d4507-114">Схема подключения для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d4507-114">Register connection schema.</span></span> |
| [<span data-ttu-id="d4507-115">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="d4507-115">Get schema</span></span>](../api/externalconnectors-schema-get.md)                        | [<span data-ttu-id="d4507-116">schema</span><span class="sxs-lookup"><span data-stu-id="d4507-116">schema</span></span>](externalconnectors-schema.md)           | <span data-ttu-id="d4507-117">Чтение свойств объекта схемы.</span><span class="sxs-lookup"><span data-stu-id="d4507-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4507-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4507-118">Properties</span></span>

| <span data-ttu-id="d4507-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4507-119">Property</span></span>   | <span data-ttu-id="d4507-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d4507-120">Type</span></span>                               | <span data-ttu-id="d4507-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4507-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="d4507-122">baseType</span><span class="sxs-lookup"><span data-stu-id="d4507-122">baseType</span></span>   | <span data-ttu-id="d4507-123">String</span><span class="sxs-lookup"><span data-stu-id="d4507-123">String</span></span>                             | <span data-ttu-id="d4507-124">Необходимо указать значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="d4507-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="d4507-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4507-125">Required.</span></span> |
| <span data-ttu-id="d4507-126">properties</span><span class="sxs-lookup"><span data-stu-id="d4507-126">properties</span></span> | <span data-ttu-id="d4507-127">[коллекция](externalconnectors-property.md) свойств</span><span class="sxs-lookup"><span data-stu-id="d4507-127">[property](externalconnectors-property.md) collection</span></span> | <span data-ttu-id="d4507-128">Свойства, определенные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="d4507-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="d4507-129">Минимальное число свойств — одно, максимальное — 128.</span><span class="sxs-lookup"><span data-stu-id="d4507-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4507-130">Связи</span><span class="sxs-lookup"><span data-stu-id="d4507-130">Relationships</span></span>

<span data-ttu-id="d4507-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d4507-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4507-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4507-132">JSON representation</span></span>

<span data-ttu-id="d4507-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4507-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
