---
title: 'СервицепринЦипалс: List ownedObjects'
description: Получение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2af06060eda49f904872dc7cc4d134db1d6dd34d
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382706"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="5e444-104">СервицепринЦипалс: List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="5e444-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="5e444-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e444-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e444-106">Получение списка объектов, принадлежащих [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5e444-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="5e444-107">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="5e444-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e444-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e444-108">Permissions</span></span>
<span data-ttu-id="5e444-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e444-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e444-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e444-111">Permission type</span></span>      | <span data-ttu-id="5e444-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e444-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e444-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e444-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5e444-114">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5e444-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e444-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e444-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e444-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e444-116">Not supported.</span></span>    |
|<span data-ttu-id="5e444-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="5e444-117">Application</span></span> | <span data-ttu-id="5e444-118">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5e444-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5e444-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e444-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e444-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e444-120">Optional query parameters</span></span>
<span data-ttu-id="5e444-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e444-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e444-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e444-122">Request headers</span></span>
| <span data-ttu-id="5e444-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5e444-123">Name</span></span>           | <span data-ttu-id="5e444-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5e444-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="5e444-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e444-125">Authorization</span></span>  | <span data-ttu-id="5e444-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e444-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e444-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e444-128">Request body</span></span>
<span data-ttu-id="5e444-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e444-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e444-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e444-130">Response</span></span>

<span data-ttu-id="5e444-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e444-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="5e444-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5e444-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="5e444-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e444-133">Request</span></span>
<span data-ttu-id="5e444-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e444-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5e444-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e444-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="5e444-136">C#</span><span class="sxs-lookup"><span data-stu-id="5e444-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e444-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e444-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e444-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e444-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e444-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e444-139">Response</span></span>
<span data-ttu-id="5e444-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e444-140">Here is an example of the response.</span></span> 
><span data-ttu-id="5e444-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e444-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
