---
title: тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1b9e3bf811807213970694ebe4e7748bf59e32ef
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467828"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="dd3c3-103">тип ресурса connectionOperation</span><span class="sxs-lookup"><span data-stu-id="dd3c3-103">connectionOperation resource type</span></span>

<span data-ttu-id="dd3c3-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="dd3c3-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3c3-105">Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) [подключения.](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="dd3c3-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dd3c3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="dd3c3-106">Methods</span></span>

| <span data-ttu-id="dd3c3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="dd3c3-107">Method</span></span>       | <span data-ttu-id="dd3c3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd3c3-108">Return Type</span></span> | <span data-ttu-id="dd3c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dd3c3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd3c3-110">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="dd3c3-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md) | [<span data-ttu-id="dd3c3-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="dd3c3-111">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="dd3c3-112">Чтение свойств объекта connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd3c3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd3c3-113">Properties</span></span>

| <span data-ttu-id="dd3c3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd3c3-114">Property</span></span> | <span data-ttu-id="dd3c3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="dd3c3-115">Type</span></span>                          | <span data-ttu-id="dd3c3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="dd3c3-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="dd3c3-117">error</span><span class="sxs-lookup"><span data-stu-id="dd3c3-117">error</span></span>    | [<span data-ttu-id="dd3c3-118">publicError</span><span class="sxs-lookup"><span data-stu-id="dd3c3-118">publicError</span></span>](publicerror.md) | <span data-ttu-id="dd3c3-119">Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="dd3c3-120">id</span><span class="sxs-lookup"><span data-stu-id="dd3c3-120">id</span></span>       | <span data-ttu-id="dd3c3-121">String</span><span class="sxs-lookup"><span data-stu-id="dd3c3-121">String</span></span>                        | <span data-ttu-id="dd3c3-122">Уникальный идентификатор для подключенияOperation.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="dd3c3-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-123">Read-only.</span></span> |
| <span data-ttu-id="dd3c3-124">status</span><span class="sxs-lookup"><span data-stu-id="dd3c3-124">status</span></span>   | <span data-ttu-id="dd3c3-125">String</span><span class="sxs-lookup"><span data-stu-id="dd3c3-125">String</span></span>                        | <span data-ttu-id="dd3c3-126">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="dd3c3-127">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd3c3-128">Связи</span><span class="sxs-lookup"><span data-stu-id="dd3c3-128">Relationships</span></span>

<span data-ttu-id="dd3c3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="dd3c3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd3c3-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd3c3-130">JSON representation</span></span>

<span data-ttu-id="dd3c3-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd3c3-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
