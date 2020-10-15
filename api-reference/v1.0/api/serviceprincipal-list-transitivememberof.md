---
title: Перечисление servicePrincipal transitive memberOf
description: Список групп и ролей каталога, участником которых является этот субъект-служба.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8f1b36106a62c5088fdb702af010599020dbfa75
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459146"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="ea68f-103">Перечисление servicePrincipal transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="ea68f-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="ea68f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea68f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea68f-105">Список групп и ролей каталога, участником которых является этот [субъект-служба](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="ea68f-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="ea68f-106">Эта операция является транзитивной и включает все группы, в которых состоит субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="ea68f-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea68f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea68f-107">Permissions</span></span>
<span data-ttu-id="ea68f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea68f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea68f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea68f-110">Permission type</span></span>      | <span data-ttu-id="ea68f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea68f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea68f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea68f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea68f-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea68f-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea68f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea68f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea68f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea68f-115">Not supported.</span></span>    |
|<span data-ttu-id="ea68f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea68f-116">Application</span></span> | <span data-ttu-id="ea68f-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea68f-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ea68f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea68f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea68f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea68f-119">Optional query parameters</span></span>
<span data-ttu-id="ea68f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea68f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea68f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea68f-121">Request headers</span></span>
| <span data-ttu-id="ea68f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ea68f-122">Name</span></span>           | <span data-ttu-id="ea68f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ea68f-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ea68f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea68f-124">Authorization</span></span>  | <span data-ttu-id="ea68f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea68f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea68f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea68f-127">Request body</span></span>
<span data-ttu-id="ea68f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea68f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea68f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea68f-129">Response</span></span>

<span data-ttu-id="ea68f-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea68f-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea68f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea68f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea68f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea68f-132">Request</span></span>

<span data-ttu-id="ea68f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea68f-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea68f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea68f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="ea68f-135">C#</span><span class="sxs-lookup"><span data-stu-id="ea68f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea68f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea68f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea68f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea68f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea68f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea68f-138">Response</span></span>

<span data-ttu-id="ea68f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea68f-139">Here is an example of the response.</span></span> 

><span data-ttu-id="ea68f-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea68f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
