---
title: Получение privilegedRole
description: 'Получение свойств и связей объекта Привилежедроле. '
localization_priority: Normal
ms.openlocfilehash: 92991de263ee573ce88d4f87345a32a3ef697d23
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594905"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="17110-103">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="17110-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17110-104">Получение свойств и связей объекта [привилежедроле](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="17110-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="17110-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17110-105">Permissions</span></span>
<span data-ttu-id="17110-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17110-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="17110-108">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="17110-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="17110-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17110-109">Permission type</span></span>      | <span data-ttu-id="17110-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17110-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17110-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17110-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17110-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17110-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17110-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17110-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17110-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17110-114">Not supported.</span></span>    |
|<span data-ttu-id="17110-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17110-115">Application</span></span> | <span data-ttu-id="17110-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17110-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17110-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17110-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17110-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17110-118">Optional query parameters</span></span>
<span data-ttu-id="17110-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17110-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17110-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17110-120">Request headers</span></span>
| <span data-ttu-id="17110-121">Имя</span><span class="sxs-lookup"><span data-stu-id="17110-121">Name</span></span>      |<span data-ttu-id="17110-122">Описание</span><span class="sxs-lookup"><span data-stu-id="17110-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17110-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17110-123">Authorization</span></span>  | <span data-ttu-id="17110-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17110-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17110-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17110-126">Request body</span></span>
<span data-ttu-id="17110-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17110-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17110-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="17110-128">Response</span></span>

<span data-ttu-id="17110-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедроле](../resources/privilegedrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17110-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="17110-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="17110-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="17110-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="17110-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="17110-132">Пример</span><span class="sxs-lookup"><span data-stu-id="17110-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17110-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="17110-133">Request</span></span>
<span data-ttu-id="17110-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17110-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="17110-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="17110-135">Response</span></span>
<span data-ttu-id="17110-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17110-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="17110-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="17110-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="17110-140">Языках</span><span class="sxs-lookup"><span data-stu-id="17110-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17110-141">Язык</span><span class="sxs-lookup"><span data-stu-id="17110-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
