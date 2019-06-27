---
title: Тип ресурса Аудитлогрут
description: Содержит различные типы журналов аудита. Эти ресурсы возвращают одноэлементный ресурс Аудитлог. Он не содержит пригодных для использования свойств.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e1b86250d933b382198a2527112b60e03f908aef
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273474"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="13e21-105">Тип ресурса Аудитлогрут</span><span class="sxs-lookup"><span data-stu-id="13e21-105">auditLogRoot resource type</span></span>

<span data-ttu-id="13e21-106">Содержит различные типы журналов аудита.</span><span class="sxs-lookup"><span data-stu-id="13e21-106">Contains different types of audit logs.</span></span> <span data-ttu-id="13e21-107">Эти ресурсы возвращают одноэлементный ресурс Аудитлог.</span><span class="sxs-lookup"><span data-stu-id="13e21-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="13e21-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="13e21-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="13e21-109">Методы</span><span class="sxs-lookup"><span data-stu-id="13e21-109">Methods</span></span>

| <span data-ttu-id="13e21-110">Метод</span><span class="sxs-lookup"><span data-stu-id="13e21-110">Method</span></span>           | <span data-ttu-id="13e21-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13e21-111">Return Type</span></span>    |<span data-ttu-id="13e21-112">Описание</span><span class="sxs-lookup"><span data-stu-id="13e21-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13e21-113">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="13e21-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="13e21-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="13e21-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="13e21-115">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="13e21-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="13e21-116">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="13e21-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="13e21-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="13e21-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="13e21-118">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="13e21-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="13e21-119">Перечисление signIn</span><span class="sxs-lookup"><span data-stu-id="13e21-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="13e21-120">signIn</span><span class="sxs-lookup"><span data-stu-id="13e21-120">signIn</span></span>](signin.md) |<span data-ttu-id="13e21-121">Чтение свойств и связей объектов signIn.</span><span class="sxs-lookup"><span data-stu-id="13e21-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="13e21-122">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="13e21-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="13e21-123">signIn</span><span class="sxs-lookup"><span data-stu-id="13e21-123">signIn</span></span>](signin.md) |<span data-ttu-id="13e21-124">Чтение свойств и связей объекта signIn.</span><span class="sxs-lookup"><span data-stu-id="13e21-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13e21-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="13e21-125">Properties</span></span>

<span data-ttu-id="13e21-126">Нет</span><span class="sxs-lookup"><span data-stu-id="13e21-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="13e21-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="13e21-127">Relationships</span></span>

| <span data-ttu-id="13e21-128">Отношение</span><span class="sxs-lookup"><span data-stu-id="13e21-128">Relationship</span></span> | <span data-ttu-id="13e21-129">Тип</span><span class="sxs-lookup"><span data-stu-id="13e21-129">Type</span></span>   |<span data-ttu-id="13e21-130">Описание</span><span class="sxs-lookup"><span data-stu-id="13e21-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e21-131">Директоряудитс</span><span class="sxs-lookup"><span data-stu-id="13e21-131">directoryAudits</span></span>|<span data-ttu-id="13e21-132">Коллекция [директоряудит](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="13e21-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="13e21-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13e21-133">Read-only.</span></span> <span data-ttu-id="13e21-134">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="13e21-134">Nullable.</span></span>|
|<span data-ttu-id="13e21-135">Сигнинс</span><span class="sxs-lookup"><span data-stu-id="13e21-135">signIns</span></span>|<span data-ttu-id="13e21-136">Коллекция [SignIn](signin.md)</span><span class="sxs-lookup"><span data-stu-id="13e21-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="13e21-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="13e21-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13e21-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13e21-139">JSON representation</span></span>

<span data-ttu-id="13e21-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13e21-140">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="13e21-141">Пример</span><span class="sxs-lookup"><span data-stu-id="13e21-141">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="13e21-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="13e21-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="13e21-143">C#</span><span class="sxs-lookup"><span data-stu-id="13e21-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13e21-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="13e21-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_auditLogs-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="13e21-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="13e21-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_auditLogs-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
