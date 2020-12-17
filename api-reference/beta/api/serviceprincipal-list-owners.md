---
title: 'servicePrincipals: Перечисление владельцев'
description: Извлечение списка владельцев servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: e0a820265a9816b235c81dfd189a1d7cdcd046c9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981168"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="39762-103">servicePrincipals: Перечисление владельцев</span><span class="sxs-lookup"><span data-stu-id="39762-103">servicePrincipals: List owners</span></span>

<span data-ttu-id="39762-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39762-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39762-105">Извлечение списка владельцев [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="39762-105">Retrieve a list of owners of the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="39762-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39762-106">Permissions</span></span>
<span data-ttu-id="39762-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39762-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39762-109">Permission type</span></span>      | <span data-ttu-id="39762-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39762-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39762-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39762-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39762-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39762-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39762-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39762-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39762-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39762-114">Not supported.</span></span>    |
|<span data-ttu-id="39762-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39762-115">Application</span></span> | <span data-ttu-id="39762-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39762-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="39762-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39762-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39762-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39762-118">Optional query parameters</span></span>
<span data-ttu-id="39762-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39762-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39762-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39762-120">Request headers</span></span>
| <span data-ttu-id="39762-121">Имя</span><span class="sxs-lookup"><span data-stu-id="39762-121">Name</span></span>           | <span data-ttu-id="39762-122">Описание</span><span class="sxs-lookup"><span data-stu-id="39762-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="39762-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39762-123">Authorization</span></span>  | <span data-ttu-id="39762-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39762-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39762-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39762-126">Request body</span></span>
<span data-ttu-id="39762-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39762-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39762-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="39762-128">Response</span></span>

<span data-ttu-id="39762-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39762-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="39762-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="39762-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="39762-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="39762-131">Request</span></span>
<span data-ttu-id="39762-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39762-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="39762-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="39762-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="39762-134">C#</span><span class="sxs-lookup"><span data-stu-id="39762-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39762-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39762-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39762-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39762-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39762-137">Java</span><span class="sxs-lookup"><span data-stu-id="39762-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39762-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="39762-138">Response</span></span>
<span data-ttu-id="39762-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39762-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="39762-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39762-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
