---
title: 'servicePrincipals: Перечисление ownedObjects'
description: Извлечение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 614d91b837bf5a275d19171271336ab5fa3faec0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134318"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="18878-104">servicePrincipals: Перечисление ownedObjects</span><span class="sxs-lookup"><span data-stu-id="18878-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="18878-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18878-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18878-106">Извлечение списка объектов, принадлежащих [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="18878-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="18878-107">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="18878-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="18878-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18878-108">Permissions</span></span>
<span data-ttu-id="18878-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18878-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18878-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18878-111">Permission type</span></span>      | <span data-ttu-id="18878-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18878-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18878-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18878-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18878-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18878-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18878-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18878-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18878-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18878-116">Not supported.</span></span>    |
|<span data-ttu-id="18878-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18878-117">Application</span></span> | <span data-ttu-id="18878-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18878-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="18878-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18878-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18878-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18878-120">Optional query parameters</span></span>
<span data-ttu-id="18878-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18878-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18878-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18878-122">Request headers</span></span>
| <span data-ttu-id="18878-123">Имя</span><span class="sxs-lookup"><span data-stu-id="18878-123">Name</span></span>           | <span data-ttu-id="18878-124">Описание</span><span class="sxs-lookup"><span data-stu-id="18878-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="18878-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18878-125">Authorization</span></span>  | <span data-ttu-id="18878-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18878-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18878-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18878-128">Request body</span></span>
<span data-ttu-id="18878-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18878-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18878-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="18878-130">Response</span></span>

<span data-ttu-id="18878-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18878-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="18878-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="18878-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="18878-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="18878-133">Request</span></span>
<span data-ttu-id="18878-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18878-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18878-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="18878-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="18878-136">C#</span><span class="sxs-lookup"><span data-stu-id="18878-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18878-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18878-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18878-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18878-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18878-139">Java</span><span class="sxs-lookup"><span data-stu-id="18878-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18878-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="18878-140">Response</span></span>
<span data-ttu-id="18878-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18878-141">Here is an example of the response.</span></span> 
><span data-ttu-id="18878-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18878-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

