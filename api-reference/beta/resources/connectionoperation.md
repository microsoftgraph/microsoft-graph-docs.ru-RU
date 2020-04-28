---
title: Тип ресурса Коннектионоператион
description: Описывает состояние асинхронного запроса для создания схемы подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21d962bbbfee64c51f11cf1ac3f5e7de2c0497e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507487"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="d50c6-103">Тип ресурса Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="d50c6-103">connectionOperation resource type</span></span>

<span data-ttu-id="d50c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d50c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d50c6-105">Описывает состояние асинхронного запроса для создания [схемы](schema.md)подключения поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="d50c6-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="d50c6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d50c6-106">Methods</span></span>

| <span data-ttu-id="d50c6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d50c6-107">Method</span></span>       | <span data-ttu-id="d50c6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d50c6-108">Return Type</span></span> | <span data-ttu-id="d50c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d50c6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d50c6-110">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="d50c6-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="d50c6-111">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="d50c6-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="d50c6-112">Чтение свойств объекта Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="d50c6-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d50c6-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="d50c6-113">Properties</span></span>

| <span data-ttu-id="d50c6-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="d50c6-114">Property</span></span> | <span data-ttu-id="d50c6-115">Тип</span><span class="sxs-lookup"><span data-stu-id="d50c6-115">Type</span></span>                          | <span data-ttu-id="d50c6-116">Описание</span><span class="sxs-lookup"><span data-stu-id="d50c6-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="d50c6-117">error</span><span class="sxs-lookup"><span data-stu-id="d50c6-117">error</span></span>    | [<span data-ttu-id="d50c6-118">еррордетаил</span><span class="sxs-lookup"><span data-stu-id="d50c6-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="d50c6-119">Если `status` это `failed`так, предоставляет дополнительные сведения об ошибке, вызвавшей сбой.</span><span class="sxs-lookup"><span data-stu-id="d50c6-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="d50c6-120">id</span><span class="sxs-lookup"><span data-stu-id="d50c6-120">id</span></span>       | <span data-ttu-id="d50c6-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d50c6-121">String</span></span>                        | <span data-ttu-id="d50c6-122">Уникальный идентификатор для Коннектионоператион.</span><span class="sxs-lookup"><span data-stu-id="d50c6-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="d50c6-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d50c6-123">Read-only.</span></span> |
| <span data-ttu-id="d50c6-124">status</span><span class="sxs-lookup"><span data-stu-id="d50c6-124">status</span></span>   | <span data-ttu-id="d50c6-125">string</span><span class="sxs-lookup"><span data-stu-id="d50c6-125">string</span></span>                        | <span data-ttu-id="d50c6-126">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d50c6-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="d50c6-127">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d50c6-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d50c6-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d50c6-128">Relationships</span></span>

<span data-ttu-id="d50c6-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d50c6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d50c6-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d50c6-130">JSON representation</span></span>

<span data-ttu-id="d50c6-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d50c6-131">The following is a JSON representation of the resource.</span></span>

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
