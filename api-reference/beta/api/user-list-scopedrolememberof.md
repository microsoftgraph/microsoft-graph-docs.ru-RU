---
title: Список Скопедадминистратороф
description: Получение списка Scopedrolemembership изменен для пользователя.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 48b8412b8646cb6daa9d802bd48a966e7d12c58a
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107579"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="4d930-103">Список Скопедадминистратороф</span><span class="sxs-lookup"><span data-stu-id="4d930-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="4d930-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d930-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d930-105">Получение списка [scopedrolemembership изменен](../resources/scopedrolemembership.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d930-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d930-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d930-106">Permissions</span></span>
<span data-ttu-id="4d930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d930-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d930-109">Permission type</span></span>      | <span data-ttu-id="4d930-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d930-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d930-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d930-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d930-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d930-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d930-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d930-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d930-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d930-114">Not supported.</span></span>    |
|<span data-ttu-id="4d930-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d930-115">Application</span></span> | <span data-ttu-id="4d930-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d930-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d930-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d930-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4d930-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d930-118">Optional query parameters</span></span>
<span data-ttu-id="4d930-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d930-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d930-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d930-120">Request headers</span></span>
| <span data-ttu-id="4d930-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d930-121">Header</span></span>       | <span data-ttu-id="4d930-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4d930-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d930-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d930-123">Authorization</span></span>  | <span data-ttu-id="4d930-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d930-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d930-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d930-126">Request body</span></span>
<span data-ttu-id="4d930-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d930-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d930-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d930-128">Response</span></span>

<span data-ttu-id="4d930-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d930-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d930-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4d930-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d930-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d930-131">Request</span></span>
<span data-ttu-id="4d930-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d930-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d930-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d930-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
# <a name="c"></a>[<span data-ttu-id="4d930-134">C#</span><span class="sxs-lookup"><span data-stu-id="4d930-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d930-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d930-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d930-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d930-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d930-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d930-137">Response</span></span>
<span data-ttu-id="4d930-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d930-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
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
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
