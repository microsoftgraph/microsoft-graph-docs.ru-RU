---
title: Список servicePrincipal memberOf
description: Получение групп и ролей каталогов, непосредственным участником которых является данный участник службы. Эта операция не является транзитивной.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 65de131fb08be8bda00e73b5bdda6eb552a80008
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383975"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="926e9-104">Список servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="926e9-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="926e9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926e9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="926e9-106">Получение групп и ролей каталогов, непосредственным участником которых является [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="926e9-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="926e9-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="926e9-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="926e9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="926e9-108">Permissions</span></span>

<span data-ttu-id="926e9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="926e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="926e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="926e9-111">Permission type</span></span>      | <span data-ttu-id="926e9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="926e9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="926e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="926e9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="926e9-114">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="926e9-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="926e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="926e9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="926e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="926e9-116">Not supported.</span></span>    |
|<span data-ttu-id="926e9-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="926e9-117">Application</span></span> | <span data-ttu-id="926e9-118">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="926e9-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="926e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="926e9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="926e9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="926e9-120">Optional query parameters</span></span>

<span data-ttu-id="926e9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="926e9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="926e9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="926e9-122">Request headers</span></span>
| <span data-ttu-id="926e9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="926e9-123">Name</span></span>           | <span data-ttu-id="926e9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="926e9-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="926e9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="926e9-125">Authorization</span></span>  | <span data-ttu-id="926e9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="926e9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="926e9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="926e9-128">Request body</span></span>
<span data-ttu-id="926e9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="926e9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="926e9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="926e9-130">Response</span></span>

<span data-ttu-id="926e9-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="926e9-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="926e9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="926e9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="926e9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="926e9-133">Request</span></span>

<span data-ttu-id="926e9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="926e9-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="926e9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="926e9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="926e9-136">C#</span><span class="sxs-lookup"><span data-stu-id="926e9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="926e9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="926e9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="926e9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="926e9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="926e9-139">Java</span><span class="sxs-lookup"><span data-stu-id="926e9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="926e9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="926e9-140">Response</span></span>

<span data-ttu-id="926e9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="926e9-141">Here is an example of the response.</span></span> 
><span data-ttu-id="926e9-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="926e9-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
