---
title: 'servicePrincipal: Перечисление createdObjects'
description: Получение списка объектов directoryobject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c5fdc6e11eeb903c86b6d872967141ec51878b2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054471"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="5a61e-103">servicePrincipal: Перечисление createdObjects</span><span class="sxs-lookup"><span data-stu-id="5a61e-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="5a61e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a61e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a61e-105">Получение списка объектов directoryobject.</span><span class="sxs-lookup"><span data-stu-id="5a61e-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a61e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a61e-106">Permissions</span></span>
<span data-ttu-id="5a61e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a61e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a61e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a61e-109">Permission type</span></span>      | <span data-ttu-id="5a61e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a61e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a61e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a61e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5a61e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a61e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a61e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a61e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a61e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a61e-114">Not supported.</span></span>    |
|<span data-ttu-id="5a61e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a61e-115">Application</span></span> | <span data-ttu-id="5a61e-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a61e-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5a61e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a61e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a61e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5a61e-118">Optional query parameters</span></span>
<span data-ttu-id="5a61e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5a61e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a61e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a61e-120">Request headers</span></span>
| <span data-ttu-id="5a61e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5a61e-121">Name</span></span>           | <span data-ttu-id="5a61e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a61e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="5a61e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a61e-123">Authorization</span></span>  | <span data-ttu-id="5a61e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a61e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a61e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a61e-126">Request body</span></span>
<span data-ttu-id="5a61e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a61e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a61e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a61e-128">Response</span></span>

<span data-ttu-id="5a61e-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a61e-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="5a61e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a61e-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="5a61e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a61e-131">Request</span></span>
<span data-ttu-id="5a61e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a61e-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a61e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a61e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="5a61e-134">C#</span><span class="sxs-lookup"><span data-stu-id="5a61e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a61e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a61e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a61e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a61e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a61e-137">Java</span><span class="sxs-lookup"><span data-stu-id="5a61e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5a61e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a61e-138">Response</span></span>
<span data-ttu-id="5a61e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a61e-139">Here is an example of the response.</span></span> <span data-ttu-id="5a61e-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5a61e-140">Note: The response object shown here might be shortened for readability.</span></span>
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
