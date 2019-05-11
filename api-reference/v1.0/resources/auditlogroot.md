---
title: Тип ресурса Аудитлогрут
description: Содержит различные типы журналов аудита. Эти ресурсы возвращают одноэлементный ресурс Аудитлог. Он не содержит пригодных для использования свойств.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 204dfbb3f03be9550429694434bcb420b93e788d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951417"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="b10af-105">Тип ресурса Аудитлогрут</span><span class="sxs-lookup"><span data-stu-id="b10af-105">auditLogRoot resource type</span></span>

<span data-ttu-id="b10af-106">Содержит различные типы журналов аудита.</span><span class="sxs-lookup"><span data-stu-id="b10af-106">Contains different types of audit logs.</span></span> <span data-ttu-id="b10af-107">Эти ресурсы возвращают одноэлементный ресурс Аудитлог.</span><span class="sxs-lookup"><span data-stu-id="b10af-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="b10af-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="b10af-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b10af-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b10af-109">Methods</span></span>

| <span data-ttu-id="b10af-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b10af-110">Method</span></span>           | <span data-ttu-id="b10af-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b10af-111">Return Type</span></span>    |<span data-ttu-id="b10af-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b10af-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b10af-113">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="b10af-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="b10af-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b10af-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="b10af-115">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="b10af-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="b10af-116">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b10af-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="b10af-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="b10af-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="b10af-118">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="b10af-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="b10af-119">Перечисление signIn</span><span class="sxs-lookup"><span data-stu-id="b10af-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="b10af-120">signIn</span><span class="sxs-lookup"><span data-stu-id="b10af-120">signIn</span></span>](signin.md) |<span data-ttu-id="b10af-121">Чтение свойств и связей объектов signIn.</span><span class="sxs-lookup"><span data-stu-id="b10af-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="b10af-122">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="b10af-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="b10af-123">signIn</span><span class="sxs-lookup"><span data-stu-id="b10af-123">signIn</span></span>](signin.md) |<span data-ttu-id="b10af-124">Чтение свойств и связей объекта signIn.</span><span class="sxs-lookup"><span data-stu-id="b10af-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b10af-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="b10af-125">Properties</span></span>

<span data-ttu-id="b10af-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b10af-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b10af-127">Связи</span><span class="sxs-lookup"><span data-stu-id="b10af-127">Relationships</span></span>

| <span data-ttu-id="b10af-128">Отношение</span><span class="sxs-lookup"><span data-stu-id="b10af-128">Relationship</span></span> | <span data-ttu-id="b10af-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b10af-129">Type</span></span>   |<span data-ttu-id="b10af-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b10af-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b10af-131">Директоряудитс</span><span class="sxs-lookup"><span data-stu-id="b10af-131">directoryAudits</span></span>|<span data-ttu-id="b10af-132">Коллекция [директоряудит](directoryAudit.md)</span><span class="sxs-lookup"><span data-stu-id="b10af-132">[directoryAudit](directoryAudit.md) collection</span></span>| <span data-ttu-id="b10af-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b10af-133">Read-only.</span></span> <span data-ttu-id="b10af-134">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b10af-134">Nullable.</span></span>|
|<span data-ttu-id="b10af-135">Сигнинс</span><span class="sxs-lookup"><span data-stu-id="b10af-135">signIns</span></span>|<span data-ttu-id="b10af-136">Коллекция [SignIn](signIn.md)</span><span class="sxs-lookup"><span data-stu-id="b10af-136">[signIn](signIn.md) collection</span></span>| <span data-ttu-id="b10af-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b10af-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b10af-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b10af-139">JSON representation</span></span>

<span data-ttu-id="b10af-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b10af-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b10af-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b10af-141">Example</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b10af-142">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="b10af-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b10af-143">C#</span><span class="sxs-lookup"><span data-stu-id="b10af-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b10af-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b10af-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_auditLogs-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
