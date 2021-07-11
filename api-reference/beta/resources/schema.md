---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6bcb5d7b10a71f6031a4215fe9f0c294c5af1840
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366942"
---
# <a name="schema-resource-type"></a><span data-ttu-id="cbcfb-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="cbcfb-103">schema resource type</span></span>

<span data-ttu-id="cbcfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbcfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbcfb-105">Схема [подключения](externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-105">The [connection](externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="cbcfb-106">Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="cbcfb-107">Перед добавлением элементов в связь вы должны зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="cbcfb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cbcfb-108">Methods</span></span>

| <span data-ttu-id="cbcfb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cbcfb-109">Method</span></span>                                                    | <span data-ttu-id="cbcfb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbcfb-110">Return Type</span></span>                   | <span data-ttu-id="cbcfb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cbcfb-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="cbcfb-112">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="cbcfb-112">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="cbcfb-113">Нет *или* [схемы](schema.md)</span><span class="sxs-lookup"><span data-stu-id="cbcfb-113">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="cbcfb-114">Схема подключения для регистрации.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-114">Register connection schema.</span></span> |
| [<span data-ttu-id="cbcfb-115">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="cbcfb-115">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="cbcfb-116">schema</span><span class="sxs-lookup"><span data-stu-id="cbcfb-116">schema</span></span>](schema.md)           | <span data-ttu-id="cbcfb-117">Чтение свойств объекта схемы.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cbcfb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbcfb-118">Properties</span></span>

| <span data-ttu-id="cbcfb-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbcfb-119">Property</span></span>   | <span data-ttu-id="cbcfb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cbcfb-120">Type</span></span>                               | <span data-ttu-id="cbcfb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cbcfb-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="cbcfb-122">baseType</span><span class="sxs-lookup"><span data-stu-id="cbcfb-122">baseType</span></span>   | <span data-ttu-id="cbcfb-123">String</span><span class="sxs-lookup"><span data-stu-id="cbcfb-123">String</span></span>                             | <span data-ttu-id="cbcfb-124">Необходимо указать значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="cbcfb-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-125">Required.</span></span> |
| <span data-ttu-id="cbcfb-126">properties</span><span class="sxs-lookup"><span data-stu-id="cbcfb-126">properties</span></span> | <span data-ttu-id="cbcfb-127">[коллекция](property.md) свойств</span><span class="sxs-lookup"><span data-stu-id="cbcfb-127">[property](property.md) collection</span></span> | <span data-ttu-id="cbcfb-128">Свойства, определенные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="cbcfb-129">Минимальное число свойств — одно, максимальное — 128.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbcfb-130">Связи</span><span class="sxs-lookup"><span data-stu-id="cbcfb-130">Relationships</span></span>

<span data-ttu-id="cbcfb-131">Нет</span><span class="sxs-lookup"><span data-stu-id="cbcfb-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbcfb-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbcfb-132">JSON representation</span></span>

<span data-ttu-id="cbcfb-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbcfb-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
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


