---
title: Перечисление registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e0e0dbafb3d77ae58e4dae111805728f2591b42f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601561"
---
# <a name="list-registereddevices"></a><span data-ttu-id="9e768-103">Перечисление registeredDevices</span><span class="sxs-lookup"><span data-stu-id="9e768-103">List registeredDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e768-104">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e768-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e768-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e768-105">Permissions</span></span>
<span data-ttu-id="9e768-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e768-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e768-108">Permission type</span></span>      | <span data-ttu-id="9e768-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e768-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e768-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e768-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e768-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e768-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e768-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e768-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e768-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e768-113">Not supported.</span></span>    |
|<span data-ttu-id="9e768-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e768-114">Application</span></span> | <span data-ttu-id="9e768-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e768-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e768-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e768-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e768-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e768-117">Optional query parameters</span></span>
<span data-ttu-id="9e768-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e768-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9e768-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e768-119">Request headers</span></span>
| <span data-ttu-id="9e768-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e768-120">Header</span></span>       | <span data-ttu-id="9e768-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9e768-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e768-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e768-122">Authorization</span></span>  | <span data-ttu-id="9e768-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e768-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9e768-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e768-125">Accept</span></span>  | <span data-ttu-id="9e768-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e768-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e768-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e768-127">Request body</span></span>
<span data-ttu-id="9e768-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e768-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e768-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e768-129">Response</span></span>

<span data-ttu-id="9e768-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e768-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e768-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e768-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e768-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e768-132">Request</span></span>
<span data-ttu-id="9e768-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e768-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="9e768-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e768-134">Response</span></span>
<span data-ttu-id="9e768-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e768-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9e768-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9e768-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9e768-139">Языках</span><span class="sxs-lookup"><span data-stu-id="9e768-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registereddevices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e768-140">Язык</span><span class="sxs-lookup"><span data-stu-id="9e768-140">Javascript</span></span>](#tab/javascript)
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
