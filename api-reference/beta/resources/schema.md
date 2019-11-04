---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8bd5d47f444d7054aecbf7b0a63e57643837a340
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938788"
---
# <a name="schema-resource-type"></a><span data-ttu-id="5c196-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="5c196-103">schema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c196-104">Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="5c196-104">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5c196-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5c196-105">Methods</span></span>

| <span data-ttu-id="5c196-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5c196-106">Method</span></span>                                                    | <span data-ttu-id="5c196-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c196-107">Return Type</span></span>                   | <span data-ttu-id="5c196-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5c196-108">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="5c196-109">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="5c196-109">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="5c196-110">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="5c196-110">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="5c196-111">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="5c196-111">Register connection schema.</span></span> |
| [<span data-ttu-id="5c196-112">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="5c196-112">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="5c196-113">схемы</span><span class="sxs-lookup"><span data-stu-id="5c196-113">schema</span></span>](schema.md)           | <span data-ttu-id="5c196-114">Чтение свойств объекта Schema.</span><span class="sxs-lookup"><span data-stu-id="5c196-114">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c196-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c196-115">Properties</span></span>

| <span data-ttu-id="5c196-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c196-116">Property</span></span>   | <span data-ttu-id="5c196-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5c196-117">Type</span></span>                               | <span data-ttu-id="5c196-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5c196-118">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="5c196-119">baseType</span><span class="sxs-lookup"><span data-stu-id="5c196-119">baseType</span></span>   | <span data-ttu-id="5c196-120">Строка</span><span class="sxs-lookup"><span data-stu-id="5c196-120">String</span></span>                             | <span data-ttu-id="5c196-121">Возможные значения: `microsoft.graph.externalItem` и `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="5c196-121">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="5c196-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="5c196-122">Required.</span></span> |
| <span data-ttu-id="5c196-123">properties</span><span class="sxs-lookup"><span data-stu-id="5c196-123">properties</span></span> | <span data-ttu-id="5c196-124">Коллекция [свойств](property.md)</span><span class="sxs-lookup"><span data-stu-id="5c196-124">[property](property.md) collection</span></span> | <span data-ttu-id="5c196-125">Свойства, заданные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="5c196-125">The properties defined for the items in the connection.</span></span> <span data-ttu-id="5c196-126">Минимальное число свойств — 1, максимальное — 64.</span><span class="sxs-lookup"><span data-stu-id="5c196-126">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="5c196-127">Является обязательным `baseType` , если задано значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="5c196-127">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="5c196-128">Игнорируется `baseType` , если задано значение `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="5c196-128">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5c196-129">Связи</span><span class="sxs-lookup"><span data-stu-id="5c196-129">Relationships</span></span>

<span data-ttu-id="5c196-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5c196-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c196-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c196-131">JSON representation</span></span>

<span data-ttu-id="5c196-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c196-132">The following is a JSON representation of the resource.</span></span>

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
