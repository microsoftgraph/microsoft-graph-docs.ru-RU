---
title: 'servicePrincipal: Перечисление createdObjects'
description: Получение списка объектов directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 23f93a48e808a72e312c55def59fae0a89d6daeb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053491"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="fb934-103">servicePrincipal: Перечисление createdObjects</span><span class="sxs-lookup"><span data-stu-id="fb934-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="fb934-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb934-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb934-105">Получение списка объектов directoryobject.</span><span class="sxs-lookup"><span data-stu-id="fb934-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb934-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb934-106">Permissions</span></span>
<span data-ttu-id="fb934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb934-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb934-109">Permission type</span></span>      | <span data-ttu-id="fb934-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb934-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb934-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb934-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb934-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb934-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb934-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb934-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb934-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb934-114">Not supported.</span></span>    |
|<span data-ttu-id="fb934-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb934-115">Application</span></span> | <span data-ttu-id="fb934-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb934-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="fb934-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb934-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb934-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb934-118">Optional query parameters</span></span>
<span data-ttu-id="fb934-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb934-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb934-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb934-120">Request headers</span></span>
| <span data-ttu-id="fb934-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fb934-121">Name</span></span>           | <span data-ttu-id="fb934-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb934-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fb934-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb934-123">Authorization</span></span>  | <span data-ttu-id="fb934-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb934-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb934-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb934-126">Request body</span></span>
<span data-ttu-id="fb934-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb934-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb934-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb934-128">Response</span></span>

<span data-ttu-id="fb934-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb934-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="fb934-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb934-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="fb934-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb934-131">Request</span></span>
<span data-ttu-id="fb934-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb934-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb934-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb934-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="fb934-134">C#</span><span class="sxs-lookup"><span data-stu-id="fb934-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb934-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb934-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb934-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb934-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb934-137">Java</span><span class="sxs-lookup"><span data-stu-id="fb934-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb934-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb934-138">Response</span></span>
<span data-ttu-id="fb934-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb934-139">Here is an example of the response.</span></span> 
><span data-ttu-id="fb934-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fb934-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

