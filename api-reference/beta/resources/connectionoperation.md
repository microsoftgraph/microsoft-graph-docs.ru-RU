---
title: Тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса на создание схемы подключения Поиска (Майкрософт).
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158305"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="5341c-103">Тип ресурса connectionOperation</span><span class="sxs-lookup"><span data-stu-id="5341c-103">connectionOperation resource type</span></span>

<span data-ttu-id="5341c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5341c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5341c-105">Описывает состояние асинхронного запроса на создание схемы подключения Поиска [(Майкрософт).](schema.md)</span><span class="sxs-lookup"><span data-stu-id="5341c-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="5341c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5341c-106">Methods</span></span>

| <span data-ttu-id="5341c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5341c-107">Method</span></span>       | <span data-ttu-id="5341c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5341c-108">Return Type</span></span> | <span data-ttu-id="5341c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5341c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5341c-110">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="5341c-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="5341c-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="5341c-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="5341c-112">Чтение свойств объекта connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="5341c-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5341c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="5341c-113">Properties</span></span>

| <span data-ttu-id="5341c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="5341c-114">Property</span></span> | <span data-ttu-id="5341c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="5341c-115">Type</span></span>                          | <span data-ttu-id="5341c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5341c-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="5341c-117">error</span><span class="sxs-lookup"><span data-stu-id="5341c-117">error</span></span>    | [<span data-ttu-id="5341c-118">errorDetail</span><span class="sxs-lookup"><span data-stu-id="5341c-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="5341c-119">Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою.</span><span class="sxs-lookup"><span data-stu-id="5341c-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="5341c-120">id</span><span class="sxs-lookup"><span data-stu-id="5341c-120">id</span></span>       | <span data-ttu-id="5341c-121">String</span><span class="sxs-lookup"><span data-stu-id="5341c-121">String</span></span>                        | <span data-ttu-id="5341c-122">Уникальный идентификатор для connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="5341c-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="5341c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5341c-123">Read-only.</span></span> |
| <span data-ttu-id="5341c-124">status</span><span class="sxs-lookup"><span data-stu-id="5341c-124">status</span></span>   | <span data-ttu-id="5341c-125">string</span><span class="sxs-lookup"><span data-stu-id="5341c-125">string</span></span>                        | <span data-ttu-id="5341c-126">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="5341c-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="5341c-127">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5341c-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5341c-128">Связи</span><span class="sxs-lookup"><span data-stu-id="5341c-128">Relationships</span></span>

<span data-ttu-id="5341c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5341c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5341c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5341c-130">JSON representation</span></span>

<span data-ttu-id="5341c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5341c-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
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


