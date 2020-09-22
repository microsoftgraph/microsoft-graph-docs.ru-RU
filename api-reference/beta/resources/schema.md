---
title: Тип ресурса схемы
description: Схема подключения определяет, как контент, добавляемый в подключение, будет использоваться в различных интерфейсах Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ff14f04adb31d99aadec15cb9368e09a098c7a26
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192870"
---
# <a name="schema-resource-type"></a><span data-ttu-id="d2a4c-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="d2a4c-103">schema resource type</span></span>

<span data-ttu-id="d2a4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a4c-105">Схема [подключения](externalconnection.md) определяет, как внешнее содержимое будет использоваться в различных интерфейсах Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-105">The [connection](externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="d2a4c-106">Schema — это плоский список всех свойств, которые вы планируете добавить к подключению вместе с их атрибутами, метками и псевдонимами.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="d2a4c-107">Перед добавлением элементов в подключение необходимо зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-107">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="d2a4c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d2a4c-108">Methods</span></span>

| <span data-ttu-id="d2a4c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d2a4c-109">Method</span></span>                                                    | <span data-ttu-id="d2a4c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2a4c-110">Return Type</span></span>                   | <span data-ttu-id="d2a4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2a4c-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="d2a4c-112">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="d2a4c-112">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="d2a4c-113">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="d2a4c-113">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="d2a4c-114">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-114">Register connection schema.</span></span> |
| [<span data-ttu-id="d2a4c-115">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="d2a4c-115">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="d2a4c-116">schema</span><span class="sxs-lookup"><span data-stu-id="d2a4c-116">schema</span></span>](schema.md)           | <span data-ttu-id="d2a4c-117">Чтение свойств объекта Schema.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2a4c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2a4c-118">Properties</span></span>

| <span data-ttu-id="d2a4c-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2a4c-119">Property</span></span>   | <span data-ttu-id="d2a4c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d2a4c-120">Type</span></span>                               | <span data-ttu-id="d2a4c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d2a4c-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="d2a4c-122">baseType</span><span class="sxs-lookup"><span data-stu-id="d2a4c-122">baseType</span></span>   | <span data-ttu-id="d2a4c-123">String</span><span class="sxs-lookup"><span data-stu-id="d2a4c-123">String</span></span>                             | <span data-ttu-id="d2a4c-124">Необходимо указать значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="d2a4c-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-125">Required.</span></span> |
| <span data-ttu-id="d2a4c-126">properties</span><span class="sxs-lookup"><span data-stu-id="d2a4c-126">properties</span></span> | <span data-ttu-id="d2a4c-127">Коллекция [свойств](property.md)</span><span class="sxs-lookup"><span data-stu-id="d2a4c-127">[property](property.md) collection</span></span> | <span data-ttu-id="d2a4c-128">Свойства, заданные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="d2a4c-129">Минимальное число свойств — 1, максимальное — 128.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d2a4c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="d2a4c-130">Relationships</span></span>

<span data-ttu-id="d2a4c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d2a4c-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2a4c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2a4c-132">JSON representation</span></span>

<span data-ttu-id="d2a4c-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2a4c-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
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


