---
title: Перечисление registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ee2fa5f1e33fabae9b22391f6b962a133a5a47b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637187"
---
# <a name="list-registereddevices"></a><span data-ttu-id="4541a-103">Перечисление registeredDevices</span><span class="sxs-lookup"><span data-stu-id="4541a-103">List registeredDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4541a-104">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="4541a-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="4541a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4541a-105">Permissions</span></span>
<span data-ttu-id="4541a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4541a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4541a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4541a-108">Permission type</span></span>      | <span data-ttu-id="4541a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4541a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4541a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4541a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4541a-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4541a-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4541a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4541a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4541a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4541a-113">Not supported.</span></span>    |
|<span data-ttu-id="4541a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4541a-114">Application</span></span> | <span data-ttu-id="4541a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4541a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4541a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4541a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4541a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4541a-117">Optional query parameters</span></span>
<span data-ttu-id="4541a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4541a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4541a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4541a-119">Request headers</span></span>
| <span data-ttu-id="4541a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4541a-120">Header</span></span>       | <span data-ttu-id="4541a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4541a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4541a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4541a-122">Authorization</span></span>  | <span data-ttu-id="4541a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4541a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4541a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4541a-125">Accept</span></span>  | <span data-ttu-id="4541a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4541a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4541a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4541a-127">Request body</span></span>
<span data-ttu-id="4541a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4541a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4541a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4541a-129">Response</span></span>

<span data-ttu-id="4541a-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4541a-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4541a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4541a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4541a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4541a-132">Request</span></span>
<span data-ttu-id="4541a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4541a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="4541a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4541a-134">Response</span></span>
<span data-ttu-id="4541a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4541a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4541a-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="4541a-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4541a-139">Языках</span><span class="sxs-lookup"><span data-stu-id="4541a-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registereddevices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4541a-140">Язык</span><span class="sxs-lookup"><span data-stu-id="4541a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registereddevices-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-registereddevices.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-registereddevices.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
