---
title: Список групп
description: Получите группы из свойства навигации групп.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2ee12f8ebc6fe5a6c300af6cfa231ee506fa38f5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873292"
---
# <a name="list-groups"></a><span data-ttu-id="62df6-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="62df6-103">List groups</span></span>
<span data-ttu-id="62df6-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="62df6-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62df6-105">Получить список объектов [группы](../resources/termstore-group.md) в [хранилище](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="62df6-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="62df6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62df6-106">Permissions</span></span>
<span data-ttu-id="62df6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62df6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62df6-109">Permission type</span></span>|<span data-ttu-id="62df6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62df6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62df6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62df6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62df6-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62df6-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="62df6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62df6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62df6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62df6-114">Not supported.</span></span>    |
|<span data-ttu-id="62df6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="62df6-115">Application</span></span> | <span data-ttu-id="62df6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62df6-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62df6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62df6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62df6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62df6-118">Optional query parameters</span></span>
<span data-ttu-id="62df6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="62df6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="62df6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="62df6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62df6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62df6-121">Request headers</span></span>
|<span data-ttu-id="62df6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="62df6-122">Name</span></span>|<span data-ttu-id="62df6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="62df6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62df6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62df6-124">Authorization</span></span>|<span data-ttu-id="62df6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62df6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62df6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62df6-127">Request body</span></span>
<span data-ttu-id="62df6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62df6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62df6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="62df6-129">Response</span></span>

<span data-ttu-id="62df6-130">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` объектов [группы](../resources/termstore-group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62df6-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62df6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="62df6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62df6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="62df6-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="62df6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="62df6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```
# <a name="c"></a>[<span data-ttu-id="62df6-134">C#</span><span class="sxs-lookup"><span data-stu-id="62df6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62df6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62df6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62df6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62df6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62df6-137">Java</span><span class="sxs-lookup"><span data-stu-id="62df6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="62df6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="62df6-138">Response</span></span>
<span data-ttu-id="62df6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62df6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.group)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "85825593-5593-8582-9355-828593558285",
      "createdDateTime": "2019-06-21T20:01:37Z",
      "description": "My term group",
      "scope" : "global",
      "displayName": "myGroup"  
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termGroups",
  "suppressions": [
  ]
}
-->



