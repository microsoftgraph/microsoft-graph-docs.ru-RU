---
title: Перечисление транзитивных servicePrincipal memberOf
description: Получение групп и ролей каталогов, членом которых является данный участник службы. Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 08abf0ba21404fe9d900784f3f54204af4ba750a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219041"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="6ab14-104">Перечисление транзитивных servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="6ab14-104">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="6ab14-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab14-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ab14-106">Получение групп и ролей каталогов, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="6ab14-106">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="6ab14-107">Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.</span><span class="sxs-lookup"><span data-stu-id="6ab14-107">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ab14-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab14-108">Permissions</span></span>
<span data-ttu-id="6ab14-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ab14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab14-111">Permission type</span></span>      | <span data-ttu-id="6ab14-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ab14-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ab14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ab14-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ab14-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ab14-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ab14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ab14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ab14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ab14-116">Not supported.</span></span>    |
|<span data-ttu-id="6ab14-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ab14-117">Application</span></span> | <span data-ttu-id="6ab14-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab14-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6ab14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ab14-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ab14-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ab14-120">Optional query parameters</span></span>
<span data-ttu-id="6ab14-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ab14-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ab14-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ab14-122">Request headers</span></span>
| <span data-ttu-id="6ab14-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6ab14-123">Name</span></span>       | <span data-ttu-id="6ab14-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab14-124">Type</span></span> | <span data-ttu-id="6ab14-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab14-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ab14-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ab14-126">Authorization</span></span>  | <span data-ttu-id="6ab14-127">string</span><span class="sxs-lookup"><span data-stu-id="6ab14-127">string</span></span>  | <span data-ttu-id="6ab14-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab14-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ab14-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ab14-130">Request body</span></span>
<span data-ttu-id="6ab14-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ab14-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ab14-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ab14-132">Response</span></span>

<span data-ttu-id="6ab14-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ab14-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab14-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6ab14-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ab14-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ab14-135">Request</span></span>

<span data-ttu-id="6ab14-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ab14-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ab14-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ab14-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6ab14-138">C#</span><span class="sxs-lookup"><span data-stu-id="6ab14-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ab14-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ab14-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ab14-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ab14-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ab14-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ab14-141">Response</span></span>

<span data-ttu-id="6ab14-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ab14-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
