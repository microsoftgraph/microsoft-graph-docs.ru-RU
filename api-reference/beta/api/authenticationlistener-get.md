---
title: Получить проверку подлинностиListener
description: Ознакомьтесь с свойствами и отношениями объекта authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e6cacb31a31963457c2e37fd9a63d1c0eeea2c6c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438486"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="75394-103">Получить проверку подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="75394-103">Get authenticationListener</span></span>

<span data-ttu-id="75394-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75394-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75394-105">Получите указанный [документ проверки подлинностиListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="75394-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="75394-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75394-106">Permissions</span></span>

<span data-ttu-id="75394-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75394-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75394-109">Permission type</span></span>|<span data-ttu-id="75394-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75394-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75394-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75394-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75394-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="75394-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="75394-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75394-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75394-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75394-114">Not supported.</span></span>|
|<span data-ttu-id="75394-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="75394-115">Application</span></span>|<span data-ttu-id="75394-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="75394-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="75394-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75394-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75394-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75394-118">Optional query parameters</span></span>

<span data-ttu-id="75394-119">Этот метод поддерживает параметр запроса OData для расширения сведений `$expand` об invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="75394-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="75394-120">Ниже приведен пример.</span><span class="sxs-lookup"><span data-stu-id="75394-120">See below for an example.</span></span> <span data-ttu-id="75394-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75394-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75394-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75394-122">Request headers</span></span>

|<span data-ttu-id="75394-123">Имя</span><span class="sxs-lookup"><span data-stu-id="75394-123">Name</span></span>|<span data-ttu-id="75394-124">Описание</span><span class="sxs-lookup"><span data-stu-id="75394-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75394-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75394-125">Authorization</span></span>|<span data-ttu-id="75394-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75394-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75394-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75394-128">Request body</span></span>

<span data-ttu-id="75394-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75394-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75394-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="75394-130">Response</span></span>

<span data-ttu-id="75394-131">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [authenticationListener](../resources/authenticationlistener.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75394-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75394-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="75394-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="75394-133">Пример 1. Получить проверку подлинностиListener по id</span><span class="sxs-lookup"><span data-stu-id="75394-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="75394-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="75394-134">Request</span></span>

<span data-ttu-id="75394-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75394-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="75394-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="75394-136">Response</span></span>

<span data-ttu-id="75394-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75394-137">The following is an example of the response.</span></span>

<span data-ttu-id="75394-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75394-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
   }
}
```

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="75394-139">Пример 2. Расширение invokeUserFlowListener для определенной проверки подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="75394-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="75394-140">В следующем примере слушатель получает по id для события onSignupStart и расширяет поток пользователей, который вызывается.</span><span class="sxs-lookup"><span data-stu-id="75394-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="75394-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="75394-141">Request</span></span>

<span data-ttu-id="75394-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75394-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="75394-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="75394-143">Response</span></span>

<span data-ttu-id="75394-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75394-144">The following is an example of the response.</span></span>

<span data-ttu-id="75394-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75394-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invokeUserFlowListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
  },
  "userFlow": {
      "id": "B2X_1_Partner",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationListener",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
