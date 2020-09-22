---
title: Удаление группы
description: Удаление объекта Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: d7214dd8bfde8f15a17bc572342ea5519244014d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974116"
---
# <a name="delete-groups"></a><span data-ttu-id="d376c-103">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="d376c-103">Delete groups</span></span>
<span data-ttu-id="d376c-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d376c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d376c-105">Удаление объекта [группы](../resources/termstore-group.md) в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="d376c-105">Delete a [group](../resources/termstore-group.md) object in the term [store].</span></span>

## <a name="permissions"></a><span data-ttu-id="d376c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d376c-106">Permissions</span></span>
<span data-ttu-id="d376c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d376c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d376c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d376c-109">Permission type</span></span>|<span data-ttu-id="d376c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d376c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d376c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d376c-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d376c-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d376c-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d376c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d376c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d376c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d376c-114">Not supported.</span></span>    |
|<span data-ttu-id="d376c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d376c-115">Application</span></span> | <span data-ttu-id="d376c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d376c-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d376c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d376c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="d376c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d376c-118">Request headers</span></span>
|<span data-ttu-id="d376c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d376c-119">Name</span></span>|<span data-ttu-id="d376c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d376c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d376c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d376c-121">Authorization</span></span>|<span data-ttu-id="d376c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d376c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d376c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d376c-124">Request body</span></span>
<span data-ttu-id="d376c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d376c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d376c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d376c-126">Response</span></span>

<span data-ttu-id="d376c-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d376c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d376c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d376c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d376c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d376c-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d376c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d376c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_from_store"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="d376c-131">C#</span><span class="sxs-lookup"><span data-stu-id="d376c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-from-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d376c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d376c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-from-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d376c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d376c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-from-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d376c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d376c-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termGroup",
  "suppressions": [
  ]
}
-->


