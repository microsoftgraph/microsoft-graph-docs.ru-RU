---
title: Тип ресурса Аудитлогрут
description: Содержит различные типы журналов аудита. Эти ресурсы возвращают одноэлементный ресурс Аудитлог. Он не содержит пригодных для использования свойств.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2956b933b5d7703300964a0d6fd2014287f5e0ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030053"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="43eba-105">Тип ресурса Аудитлогрут</span><span class="sxs-lookup"><span data-stu-id="43eba-105">auditLogRoot resource type</span></span>

<span data-ttu-id="43eba-106">Содержит различные типы журналов аудита.</span><span class="sxs-lookup"><span data-stu-id="43eba-106">Contains different types of audit logs.</span></span> <span data-ttu-id="43eba-107">Эти ресурсы возвращают одноэлементный ресурс Аудитлог.</span><span class="sxs-lookup"><span data-stu-id="43eba-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="43eba-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="43eba-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="43eba-109">Методы</span><span class="sxs-lookup"><span data-stu-id="43eba-109">Methods</span></span>

| <span data-ttu-id="43eba-110">Метод</span><span class="sxs-lookup"><span data-stu-id="43eba-110">Method</span></span>           | <span data-ttu-id="43eba-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="43eba-111">Return Type</span></span>    |<span data-ttu-id="43eba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="43eba-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43eba-113">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="43eba-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="43eba-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="43eba-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="43eba-115">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="43eba-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="43eba-116">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="43eba-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="43eba-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="43eba-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="43eba-118">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="43eba-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="43eba-119">Перечисление signIn</span><span class="sxs-lookup"><span data-stu-id="43eba-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="43eba-120">signIn</span><span class="sxs-lookup"><span data-stu-id="43eba-120">signIn</span></span>](signin.md) |<span data-ttu-id="43eba-121">Чтение свойств и связей объектов signIn.</span><span class="sxs-lookup"><span data-stu-id="43eba-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="43eba-122">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="43eba-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="43eba-123">signIn</span><span class="sxs-lookup"><span data-stu-id="43eba-123">signIn</span></span>](signin.md) |<span data-ttu-id="43eba-124">Чтение свойств и связей объекта signIn.</span><span class="sxs-lookup"><span data-stu-id="43eba-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43eba-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="43eba-125">Properties</span></span>

<span data-ttu-id="43eba-126">Нет</span><span class="sxs-lookup"><span data-stu-id="43eba-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="43eba-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="43eba-127">Relationships</span></span>

| <span data-ttu-id="43eba-128">Отношение</span><span class="sxs-lookup"><span data-stu-id="43eba-128">Relationship</span></span> | <span data-ttu-id="43eba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="43eba-129">Type</span></span>   |<span data-ttu-id="43eba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="43eba-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43eba-131">Директоряудитс</span><span class="sxs-lookup"><span data-stu-id="43eba-131">directoryAudits</span></span>|<span data-ttu-id="43eba-132">Коллекция [директоряудит](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="43eba-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="43eba-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43eba-133">Read-only.</span></span> <span data-ttu-id="43eba-134">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="43eba-134">Nullable.</span></span>|
|<span data-ttu-id="43eba-135">Сигнинс</span><span class="sxs-lookup"><span data-stu-id="43eba-135">signIns</span></span>|<span data-ttu-id="43eba-136">Коллекция [SignIn](signin.md)</span><span class="sxs-lookup"><span data-stu-id="43eba-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="43eba-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="43eba-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43eba-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43eba-139">JSON representation</span></span>

<span data-ttu-id="43eba-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43eba-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="43eba-141">Пример</span><span class="sxs-lookup"><span data-stu-id="43eba-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="43eba-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="43eba-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43eba-143">C#</span><span class="sxs-lookup"><span data-stu-id="43eba-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43eba-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="43eba-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43eba-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="43eba-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="43eba-146">Java</span><span class="sxs-lookup"><span data-stu-id="43eba-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
