---
title: Получение privilegedRoleAssignment
description: Получение свойств и связей объекта Привилежедролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 1ebdf020fc3f534ec62edb345748869bd46f42d4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594671"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="5655b-103">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5655b-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5655b-104">Получение свойств и связей объекта Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="5655b-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5655b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5655b-105">Permissions</span></span>
<span data-ttu-id="5655b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5655b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5655b-108">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="5655b-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="5655b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5655b-109">Permission type</span></span>      | <span data-ttu-id="5655b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5655b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5655b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5655b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5655b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5655b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5655b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5655b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5655b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5655b-114">Not supported.</span></span>    |
|<span data-ttu-id="5655b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5655b-115">Application</span></span> | <span data-ttu-id="5655b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5655b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5655b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5655b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5655b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5655b-118">Optional query parameters</span></span>
<span data-ttu-id="5655b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5655b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5655b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5655b-120">Request headers</span></span>
| <span data-ttu-id="5655b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5655b-121">Name</span></span>      |<span data-ttu-id="5655b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5655b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5655b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5655b-123">Authorization</span></span>  | <span data-ttu-id="5655b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5655b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5655b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5655b-126">Request body</span></span>
<span data-ttu-id="5655b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5655b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5655b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5655b-128">Response</span></span>

<span data-ttu-id="5655b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5655b-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="5655b-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="5655b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5655b-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="5655b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5655b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5655b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5655b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5655b-133">Request</span></span>
<span data-ttu-id="5655b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5655b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="5655b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5655b-135">Response</span></span>
<span data-ttu-id="5655b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5655b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5655b-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5655b-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5655b-140">Языках</span><span class="sxs-lookup"><span data-stu-id="5655b-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5655b-141">Язык</span><span class="sxs-lookup"><span data-stu-id="5655b-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
