---
title: Создание identityApiConnector
description: Создание нового объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e2ff03ae081a1d406a56c5a826664bb402983a4f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435630"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="cebb6-103">Создание identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="cebb6-103">Create identityApiConnector</span></span>

<span data-ttu-id="cebb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cebb6-105">Создание нового [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="cebb6-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebb6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cebb6-106">Permissions</span></span>

<span data-ttu-id="cebb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cebb6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cebb6-109">Permission type</span></span>                        | <span data-ttu-id="cebb6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cebb6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cebb6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cebb6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cebb6-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebb6-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="cebb6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cebb6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebb6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebb6-114">Not supported.</span></span>  |
| <span data-ttu-id="cebb6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cebb6-115">Application</span></span>                            | <span data-ttu-id="cebb6-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebb6-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="cebb6-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="cebb6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="cebb6-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="cebb6-118">Global administrator</span></span>
* <span data-ttu-id="cebb6-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="cebb6-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="cebb6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cebb6-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="cebb6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cebb6-121">Request headers</span></span>

| <span data-ttu-id="cebb6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cebb6-122">Name</span></span>          | <span data-ttu-id="cebb6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cebb6-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="cebb6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cebb6-124">Authorization</span></span> | <span data-ttu-id="cebb6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cebb6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cebb6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cebb6-127">Content-Type</span></span>  | <span data-ttu-id="cebb6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cebb6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cebb6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cebb6-130">Request body</span></span>

<span data-ttu-id="cebb6-131">В теле запроса поставляем представление JSON объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="cebb6-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="cebb6-132">В следующей таблице показаны свойства, необходимые при создании [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="cebb6-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="cebb6-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="cebb6-133">Property</span></span>|<span data-ttu-id="cebb6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="cebb6-134">Type</span></span>|<span data-ttu-id="cebb6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cebb6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cebb6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cebb6-136">displayName</span></span>|<span data-ttu-id="cebb6-137">String</span><span class="sxs-lookup"><span data-stu-id="cebb6-137">String</span></span>| <span data-ttu-id="cebb6-138">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="cebb6-138">The name of the API connector.</span></span> |
|<span data-ttu-id="cebb6-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="cebb6-139">targetUrl</span></span>|<span data-ttu-id="cebb6-140">String</span><span class="sxs-lookup"><span data-stu-id="cebb6-140">String</span></span>| <span data-ttu-id="cebb6-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="cebb6-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="cebb6-142">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="cebb6-142">authenticationConfiguration</span></span>|[<span data-ttu-id="cebb6-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="cebb6-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="cebb6-144">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="cebb6-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="cebb6-145">Поддерживается [только базовая](../resources/basicauthentication.md) проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="cebb6-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="cebb6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebb6-146">Response</span></span>

<span data-ttu-id="cebb6-147">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cebb6-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cebb6-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="cebb6-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cebb6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="cebb6-149">Request</span></span>

<span data-ttu-id="cebb6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cebb6-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cebb6-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cebb6-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="cebb6-152">C#</span><span class="sxs-lookup"><span data-stu-id="cebb6-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cebb6-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cebb6-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cebb6-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cebb6-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cebb6-155">Java</span><span class="sxs-lookup"><span data-stu-id="cebb6-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cebb6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebb6-156">Response</span></span>

<span data-ttu-id="cebb6-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cebb6-157">The following is an example of the response.</span></span>

<span data-ttu-id="cebb6-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cebb6-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
