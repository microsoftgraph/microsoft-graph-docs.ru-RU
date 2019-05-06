---
title: Список групп устройств
description: Получение групп, непосредственным участником которых является это устройство. Эта операция не является транзитивной.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 767f99f83f82f394a0fb0e10111020fd5af4eea1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590990"
---
# <a name="list-device-groups"></a><span data-ttu-id="f7c6c-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="f7c6c-104">List device groups</span></span>

<span data-ttu-id="f7c6c-105">Получение групп, непосредственным участником которых является это устройство.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="f7c6c-106">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c6c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c6c-107">Permissions</span></span>

<span data-ttu-id="f7c6c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c6c-110">Permission type</span></span>      | <span data-ttu-id="f7c6c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7c6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7c6c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7c6c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7c6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-115">Not supported.</span></span>    |
|<span data-ttu-id="f7c6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c6c-116">Application</span></span> | <span data-ttu-id="f7c6c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c6c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7c6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7c6c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7c6c-119">Optional query parameters</span></span>
<span data-ttu-id="f7c6c-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f7c6c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c6c-121">Request headers</span></span>
| <span data-ttu-id="f7c6c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7c6c-122">Header</span></span>       | <span data-ttu-id="f7c6c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7c6c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7c6c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7c6c-124">Authorization</span></span>  | <span data-ttu-id="f7c6c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7c6c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f7c6c-127">Accept</span></span>  | <span data-ttu-id="f7c6c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c6c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c6c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c6c-129">Request body</span></span>
<span data-ttu-id="f7c6c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7c6c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c6c-131">Response</span></span>

<span data-ttu-id="f7c6c-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c6c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c6c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c6c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c6c-134">Request</span></span>

<span data-ttu-id="f7c6c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="f7c6c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c6c-136">Response</span></span>
<span data-ttu-id="f7c6c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c6c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7c6c-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f7c6c-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7c6c-141">Языках</span><span class="sxs-lookup"><span data-stu-id="f7c6c-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_user_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7c6c-142">Язык</span><span class="sxs-lookup"><span data-stu-id="f7c6c-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_user_memberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
