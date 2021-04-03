---
title: List identityApiConnectors
description: Получить список объектов identityApiConnector и их свойств
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6aa2d3a4a5c45dc7b9e0b168eac7402404fcb982
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507856"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="be285-103">List identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="be285-103">List identityApiConnectors</span></span>

<span data-ttu-id="be285-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be285-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be285-105">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="be285-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be285-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be285-106">Permissions</span></span>

<span data-ttu-id="be285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be285-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be285-109">Permission type</span></span>                        | <span data-ttu-id="be285-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be285-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="be285-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be285-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be285-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be285-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="be285-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be285-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be285-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be285-114">Not supported.</span></span>  |
| <span data-ttu-id="be285-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="be285-115">Application</span></span>                            | <span data-ttu-id="be285-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be285-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="be285-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="be285-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="be285-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="be285-118">Global administrator</span></span>
* <span data-ttu-id="be285-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="be285-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="be285-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be285-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be285-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be285-121">Optional query parameters</span></span>
<span data-ttu-id="be285-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="be285-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be285-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="be285-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be285-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be285-124">Request headers</span></span>
|<span data-ttu-id="be285-125">Имя</span><span class="sxs-lookup"><span data-stu-id="be285-125">Name</span></span>|<span data-ttu-id="be285-126">Описание</span><span class="sxs-lookup"><span data-stu-id="be285-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be285-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be285-127">Authorization</span></span>|<span data-ttu-id="be285-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be285-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be285-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be285-130">Request body</span></span>
<span data-ttu-id="be285-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be285-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be285-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="be285-132">Response</span></span>

<span data-ttu-id="be285-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="be285-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be285-134">Пример</span><span class="sxs-lookup"><span data-stu-id="be285-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="be285-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="be285-135">Request</span></span>

<span data-ttu-id="be285-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be285-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be285-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="be285-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="be285-138">C#</span><span class="sxs-lookup"><span data-stu-id="be285-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be285-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be285-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be285-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be285-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be285-141">Java</span><span class="sxs-lookup"><span data-stu-id="be285-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be285-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="be285-142">Response</span></span>

<span data-ttu-id="be285-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="be285-143">The following is an example of the response.</span></span>

<span data-ttu-id="be285-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="be285-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
        {
            "id": "<guid>",
            "displayName": "Test API",
            "targetUrl": "https://someapi.com/api/endpoint",
            "authenticationConfiguration": {
              "@odata.type": "#microsoft.graph.basicAuthentication",
              "username": "<USERNAME>",
              "password": "******"
            }
        },
        {
            "id": "<guid>",
            "displayName": "My API connector",
            "targetUrl": "https://someotherapi.com/api/endpoint",
            "authenticationConfiguration": {
                "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
                "certificateList": [
                    {
                        "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                        "notAfter": 1666350522,
                        "notBefore": 1508670522,
                        "isActive": true
                    },
                    {
                        "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                        "notAfter": 1766350522,
                        "notBefore": 1608670522,
                        "isActive": false
                    }
                ]
            }
        }
  ]
}
```
