---
title: тип ресурсов auditLogRoot
description: Содержит различные типы журналов аудита. Эти ресурсы возвращают однотонный ресурс auditLog. Он не содержит никаких полезных свойств.
author: dhanyahk
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 363d3a0c3aafbbd5b3d53914748dfdb1fd432b1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759729"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="a6456-105">тип ресурсов auditLogRoot</span><span class="sxs-lookup"><span data-stu-id="a6456-105">auditLogRoot resource type</span></span>

<span data-ttu-id="a6456-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6456-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6456-107">Содержит различные типы журналов аудита.</span><span class="sxs-lookup"><span data-stu-id="a6456-107">Contains different types of audit logs.</span></span> <span data-ttu-id="a6456-108">Эти ресурсы возвращают однотонный ресурс auditLog.</span><span class="sxs-lookup"><span data-stu-id="a6456-108">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="a6456-109">Он не содержит никаких полезных свойств.</span><span class="sxs-lookup"><span data-stu-id="a6456-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a6456-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a6456-110">Methods</span></span>

| <span data-ttu-id="a6456-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a6456-111">Method</span></span>           | <span data-ttu-id="a6456-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6456-112">Return Type</span></span>    |<span data-ttu-id="a6456-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a6456-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6456-114">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="a6456-114">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="a6456-115">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a6456-115">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="a6456-116">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="a6456-116">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="a6456-117">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a6456-117">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="a6456-118">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a6456-118">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="a6456-119">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="a6456-119">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="a6456-120">Перечисление signIn</span><span class="sxs-lookup"><span data-stu-id="a6456-120">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="a6456-121">signIn</span><span class="sxs-lookup"><span data-stu-id="a6456-121">signIn</span></span>](signin.md) |<span data-ttu-id="a6456-122">Чтение свойств и связей объектов signIn.</span><span class="sxs-lookup"><span data-stu-id="a6456-122">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="a6456-123">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="a6456-123">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="a6456-124">signIn</span><span class="sxs-lookup"><span data-stu-id="a6456-124">signIn</span></span>](signin.md) |<span data-ttu-id="a6456-125">Чтение свойств и связей объекта signIn.</span><span class="sxs-lookup"><span data-stu-id="a6456-125">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6456-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6456-126">Properties</span></span>

<span data-ttu-id="a6456-127">Нет</span><span class="sxs-lookup"><span data-stu-id="a6456-127">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a6456-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a6456-128">Relationships</span></span>

| <span data-ttu-id="a6456-129">Связь</span><span class="sxs-lookup"><span data-stu-id="a6456-129">Relationship</span></span> | <span data-ttu-id="a6456-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a6456-130">Type</span></span>   |<span data-ttu-id="a6456-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a6456-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6456-132">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="a6456-132">directoryAudits</span></span>|<span data-ttu-id="a6456-133">[коллекция directoryAudit](directoryaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a6456-133">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="a6456-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6456-134">Read-only.</span></span> <span data-ttu-id="a6456-135">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6456-135">Nullable.</span></span>|
|<span data-ttu-id="a6456-136">signIns</span><span class="sxs-lookup"><span data-stu-id="a6456-136">signIns</span></span>|<span data-ttu-id="a6456-137">[signIn](signin.md) collection</span><span class="sxs-lookup"><span data-stu-id="a6456-137">[signIn](signin.md) collection</span></span>| <span data-ttu-id="a6456-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6456-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6456-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6456-140">JSON representation</span></span>

<span data-ttu-id="a6456-141">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6456-141">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a6456-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a6456-142">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="a6456-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6456-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="c"></a>[<span data-ttu-id="a6456-144">C#</span><span class="sxs-lookup"><span data-stu-id="a6456-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6456-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6456-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6456-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6456-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6456-147">Java</span><span class="sxs-lookup"><span data-stu-id="a6456-147">Java</span></span>](#tab/java)
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

