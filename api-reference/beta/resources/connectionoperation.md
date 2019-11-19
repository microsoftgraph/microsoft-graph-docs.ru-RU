---
title: Тип ресурса Коннектионоператион
description: Описывает состояние асинхронного запроса для создания схемы подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9ced1c9bd00e3e865c3663ed6ade936747b9dded
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704145"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="1d684-103">Тип ресурса Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="1d684-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d684-104">Описывает состояние асинхронного запроса для создания [схемы](schema.md)подключения поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="1d684-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="1d684-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1d684-105">Methods</span></span>

| <span data-ttu-id="1d684-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1d684-106">Method</span></span>       | <span data-ttu-id="1d684-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d684-107">Return Type</span></span> | <span data-ttu-id="1d684-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1d684-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1d684-109">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="1d684-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="1d684-110">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="1d684-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="1d684-111">Чтение свойств объекта Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="1d684-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d684-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d684-112">Properties</span></span>

| <span data-ttu-id="1d684-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d684-113">Property</span></span> | <span data-ttu-id="1d684-114">Тип</span><span class="sxs-lookup"><span data-stu-id="1d684-114">Type</span></span>                          | <span data-ttu-id="1d684-115">Описание</span><span class="sxs-lookup"><span data-stu-id="1d684-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="1d684-116">error</span><span class="sxs-lookup"><span data-stu-id="1d684-116">error</span></span>    | [<span data-ttu-id="1d684-117">еррордетаил</span><span class="sxs-lookup"><span data-stu-id="1d684-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="1d684-118">Если `status` это `failed`так, предоставляет дополнительные сведения об ошибке, вызвавшей сбой.</span><span class="sxs-lookup"><span data-stu-id="1d684-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="1d684-119">id</span><span class="sxs-lookup"><span data-stu-id="1d684-119">id</span></span>       | <span data-ttu-id="1d684-120">Строка</span><span class="sxs-lookup"><span data-stu-id="1d684-120">String</span></span>                        | <span data-ttu-id="1d684-121">Уникальный идентификатор для Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="1d684-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="1d684-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d684-122">Read-only.</span></span> |
| <span data-ttu-id="1d684-123">status</span><span class="sxs-lookup"><span data-stu-id="1d684-123">status</span></span>   | <span data-ttu-id="1d684-124">string</span><span class="sxs-lookup"><span data-stu-id="1d684-124">string</span></span>                        | <span data-ttu-id="1d684-125">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="1d684-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="1d684-126">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1d684-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d684-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1d684-127">Relationships</span></span>

<span data-ttu-id="1d684-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1d684-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d684-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d684-129">JSON representation</span></span>

<span data-ttu-id="1d684-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d684-130">The following is a JSON representation of the resource.</span></span>

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
