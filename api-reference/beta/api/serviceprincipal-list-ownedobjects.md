---
title: 'servicePrincipals: Перечисление ownedObjects'
description: Извлечение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fbb61ab1fd37c8bf322b144974eee7b799bf6650
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051888"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="eda13-104">servicePrincipals: Перечисление ownedObjects</span><span class="sxs-lookup"><span data-stu-id="eda13-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="eda13-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eda13-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eda13-106">Извлечение списка объектов, принадлежащих [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="eda13-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="eda13-107">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="eda13-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="eda13-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eda13-108">Permissions</span></span>
<span data-ttu-id="eda13-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda13-111">Permission type</span></span>      | <span data-ttu-id="eda13-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda13-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eda13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda13-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eda13-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eda13-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eda13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eda13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda13-116">Not supported.</span></span>    |
|<span data-ttu-id="eda13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda13-117">Application</span></span> | <span data-ttu-id="eda13-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda13-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="eda13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda13-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eda13-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eda13-120">Optional query parameters</span></span>
<span data-ttu-id="eda13-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eda13-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eda13-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda13-122">Request headers</span></span>
| <span data-ttu-id="eda13-123">Имя</span><span class="sxs-lookup"><span data-stu-id="eda13-123">Name</span></span>           | <span data-ttu-id="eda13-124">Описание</span><span class="sxs-lookup"><span data-stu-id="eda13-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="eda13-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eda13-125">Authorization</span></span>  | <span data-ttu-id="eda13-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda13-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eda13-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda13-128">Request body</span></span>
<span data-ttu-id="eda13-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eda13-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eda13-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda13-130">Response</span></span>

<span data-ttu-id="eda13-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eda13-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="eda13-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="eda13-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="eda13-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda13-133">Request</span></span>
<span data-ttu-id="eda13-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda13-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eda13-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eda13-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="eda13-136">C#</span><span class="sxs-lookup"><span data-stu-id="eda13-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eda13-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eda13-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eda13-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eda13-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eda13-139">Java</span><span class="sxs-lookup"><span data-stu-id="eda13-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eda13-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda13-140">Response</span></span>
<span data-ttu-id="eda13-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eda13-141">Here is an example of the response.</span></span> 
><span data-ttu-id="eda13-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eda13-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

