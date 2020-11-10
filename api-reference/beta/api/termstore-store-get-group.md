---
title: Вывод группы
description: Чтение свойств и связей объекта Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: aef088e26496e7b35b14a9250725a6eaac96eb5b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972356"
---
# <a name="get-group"></a><span data-ttu-id="42ac9-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="42ac9-103">Get group</span></span>
<span data-ttu-id="42ac9-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="42ac9-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42ac9-105">Чтение свойств и связей объекта [Group](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="42ac9-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42ac9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42ac9-106">Permissions</span></span>
<span data-ttu-id="42ac9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42ac9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42ac9-109">Permission type</span></span>|<span data-ttu-id="42ac9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42ac9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42ac9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42ac9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42ac9-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42ac9-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="42ac9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42ac9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42ac9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42ac9-114">Not supported.</span></span>    |
|<span data-ttu-id="42ac9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42ac9-115">Application</span></span> | <span data-ttu-id="42ac9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42ac9-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="42ac9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42ac9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="42ac9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42ac9-118">Request headers</span></span>
|<span data-ttu-id="42ac9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="42ac9-119">Name</span></span>|<span data-ttu-id="42ac9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="42ac9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42ac9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42ac9-121">Authorization</span></span>|<span data-ttu-id="42ac9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42ac9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42ac9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42ac9-124">Request body</span></span>
<span data-ttu-id="42ac9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42ac9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42ac9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="42ac9-126">Response</span></span>

<span data-ttu-id="42ac9-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/termstore-group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42ac9-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42ac9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="42ac9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42ac9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="42ac9-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="42ac9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="42ac9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="42ac9-131">C#</span><span class="sxs-lookup"><span data-stu-id="42ac9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42ac9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42ac9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42ac9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42ac9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42ac9-134">Java</span><span class="sxs-lookup"><span data-stu-id="42ac9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="42ac9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="42ac9-135">Response</span></span>

<span data-ttu-id="42ac9-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42ac9-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup"  
}
```

[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termGroup",
  "suppressions": [
  ]
}
-->


