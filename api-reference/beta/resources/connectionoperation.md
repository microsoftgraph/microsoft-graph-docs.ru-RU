---
title: Тип ресурса Коннектионоператион
description: Описывает состояние асинхронного запроса для создания схемы подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 657d71dc6b1671b2af6011778c0b14bb299e3cf9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938886"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="b481d-103">Тип ресурса Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="b481d-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b481d-104">Описывает состояние асинхронного запроса для создания [схемы](schema.md)подключения поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="b481d-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b481d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b481d-105">Methods</span></span>

| <span data-ttu-id="b481d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b481d-106">Method</span></span>       | <span data-ttu-id="b481d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b481d-107">Return Type</span></span> | <span data-ttu-id="b481d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b481d-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b481d-109">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="b481d-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="b481d-110">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="b481d-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="b481d-111">Чтение свойств объекта Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="b481d-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b481d-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b481d-112">Properties</span></span>

| <span data-ttu-id="b481d-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b481d-113">Property</span></span> | <span data-ttu-id="b481d-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b481d-114">Type</span></span>                          | <span data-ttu-id="b481d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b481d-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="b481d-116">error</span><span class="sxs-lookup"><span data-stu-id="b481d-116">error</span></span>    | [<span data-ttu-id="b481d-117">еррордетаил</span><span class="sxs-lookup"><span data-stu-id="b481d-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="b481d-118">Если `status` это `failed`так, предоставляет дополнительные сведения об ошибке, вызвавшей сбой.</span><span class="sxs-lookup"><span data-stu-id="b481d-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="b481d-119">id</span><span class="sxs-lookup"><span data-stu-id="b481d-119">id</span></span>       | <span data-ttu-id="b481d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b481d-120">String</span></span>                        | <span data-ttu-id="b481d-121">Уникальный идентификатор для Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="b481d-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="b481d-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b481d-122">Read-only.</span></span> |
| <span data-ttu-id="b481d-123">status</span><span class="sxs-lookup"><span data-stu-id="b481d-123">status</span></span>   | <span data-ttu-id="b481d-124">string</span><span class="sxs-lookup"><span data-stu-id="b481d-124">string</span></span>                        | <span data-ttu-id="b481d-125">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="b481d-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="b481d-126">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b481d-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b481d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="b481d-127">Relationships</span></span>

<span data-ttu-id="b481d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b481d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b481d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b481d-129">JSON representation</span></span>

<span data-ttu-id="b481d-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b481d-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "",
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
