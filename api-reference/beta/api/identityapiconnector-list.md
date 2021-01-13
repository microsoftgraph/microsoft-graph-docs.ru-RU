---
title: Список identityApiConnectors
description: Получить список объектов identityApiConnector и их свойств
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd656bad651511b897c687bbca8cead22a4accc3
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844299"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="0ca35-103">Список identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="0ca35-103">List identityApiConnectors</span></span>

<span data-ttu-id="0ca35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ca35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca35-105">Чтение свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="0ca35-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ca35-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca35-106">Permissions</span></span>

<span data-ttu-id="0ca35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ca35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ca35-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca35-109">Permission type</span></span>                        | <span data-ttu-id="0ca35-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ca35-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="0ca35-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ca35-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ca35-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca35-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="0ca35-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ca35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ca35-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca35-114">Not supported.</span></span>  |
| <span data-ttu-id="0ca35-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ca35-115">Application</span></span>                            | <span data-ttu-id="0ca35-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca35-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="0ca35-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0ca35-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0ca35-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0ca35-118">Global administrator</span></span>
* <span data-ttu-id="0ca35-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="0ca35-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0ca35-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ca35-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ca35-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ca35-121">Optional query parameters</span></span>
<span data-ttu-id="0ca35-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0ca35-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0ca35-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0ca35-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ca35-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ca35-124">Request headers</span></span>
|<span data-ttu-id="0ca35-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0ca35-125">Name</span></span>|<span data-ttu-id="0ca35-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca35-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ca35-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ca35-127">Authorization</span></span>|<span data-ttu-id="0ca35-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ca35-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca35-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ca35-130">Request body</span></span>
<span data-ttu-id="0ca35-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ca35-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ca35-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca35-132">Response</span></span>

<span data-ttu-id="0ca35-133">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [identityApiConnector](../resources/identityapiconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ca35-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca35-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0ca35-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ca35-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ca35-135">Request</span></span>

<span data-ttu-id="0ca35-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ca35-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ca35-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ca35-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="0ca35-138">C#</span><span class="sxs-lookup"><span data-stu-id="0ca35-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ca35-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ca35-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ca35-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ca35-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ca35-141">Java</span><span class="sxs-lookup"><span data-stu-id="0ca35-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ca35-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca35-142">Response</span></span>

<span data-ttu-id="0ca35-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ca35-143">The following is an example of the response.</span></span>

<span data-ttu-id="0ca35-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ca35-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      }
  ]
}
```
