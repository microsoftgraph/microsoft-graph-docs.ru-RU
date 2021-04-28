---
title: Получение объекта DirectoryObject
description: Получение свойств и связей объекта directoryObject.
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ae93f6b665a8b4d6ce4ccb1c039302575e18a8f7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051503"
---
# <a name="get-directoryobject"></a><span data-ttu-id="de6b1-103">Получение объекта DirectoryObject</span><span class="sxs-lookup"><span data-stu-id="de6b1-103">Get directoryObject</span></span>

<span data-ttu-id="de6b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de6b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de6b1-105">Получение свойств и связей объекта directoryObject.</span><span class="sxs-lookup"><span data-stu-id="de6b1-105">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de6b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b1-106">Permissions</span></span>
<span data-ttu-id="de6b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b1-109">Permission type</span></span>      | <span data-ttu-id="de6b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de6b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de6b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de6b1-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de6b1-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de6b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de6b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6b1-114">Not supported.</span></span>    |
|<span data-ttu-id="de6b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de6b1-115">Application</span></span> | <span data-ttu-id="de6b1-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="de6b1-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de6b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de6b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de6b1-118">Optional query parameters</span></span>
<span data-ttu-id="de6b1-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="de6b1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de6b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de6b1-120">Request headers</span></span>
| <span data-ttu-id="de6b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="de6b1-121">Name</span></span>       | <span data-ttu-id="de6b1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="de6b1-122">Type</span></span> | <span data-ttu-id="de6b1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="de6b1-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de6b1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="de6b1-124">Authorization</span></span>  | <span data-ttu-id="de6b1-125">string</span><span class="sxs-lookup"><span data-stu-id="de6b1-125">string</span></span>  | <span data-ttu-id="de6b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de6b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de6b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de6b1-128">Request body</span></span>
<span data-ttu-id="de6b1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de6b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de6b1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="de6b1-130">Response</span></span>

<span data-ttu-id="de6b1-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de6b1-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de6b1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="de6b1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de6b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="de6b1-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="de6b1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="de6b1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="de6b1-135">C#</span><span class="sxs-lookup"><span data-stu-id="de6b1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de6b1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de6b1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de6b1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de6b1-138">Java</span><span class="sxs-lookup"><span data-stu-id="de6b1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="de6b1-139">Response</span></span>
<span data-ttu-id="de6b1-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de6b1-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
