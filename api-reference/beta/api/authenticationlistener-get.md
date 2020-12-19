---
title: Get authenticationListener
description: Чтение свойств и связей объекта authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16b31fd16d8df5e179c38a26efc47876d809d13f
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720300"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="1f3c8-103">Get authenticationListener</span><span class="sxs-lookup"><span data-stu-id="1f3c8-103">Get authenticationListener</span></span>

<span data-ttu-id="1f3c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f3c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f3c8-105">Получите указанный [authenticationListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f3c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f3c8-106">Permissions</span></span>

<span data-ttu-id="1f3c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f3c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f3c8-109">Permission type</span></span>|<span data-ttu-id="1f3c8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f3c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f3c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f3c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f3c8-112">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f3c8-112">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span></span>|
|<span data-ttu-id="1f3c8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f3c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f3c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-114">Not supported.</span></span>|
|<span data-ttu-id="1f3c8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f3c8-115">Application</span></span>|<span data-ttu-id="1f3c8-116">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f3c8-116">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f3c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f3c8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f3c8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f3c8-118">Optional query parameters</span></span>

<span data-ttu-id="1f3c8-119">Этот метод поддерживает параметр запроса OData для расширения сведений `$expand` об invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="1f3c8-120">Пример см. ниже.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-120">See below for an example.</span></span> <span data-ttu-id="1f3c8-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f3c8-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f3c8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f3c8-122">Request headers</span></span>

|<span data-ttu-id="1f3c8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1f3c8-123">Name</span></span>|<span data-ttu-id="1f3c8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1f3c8-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f3c8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f3c8-125">Authorization</span></span>|<span data-ttu-id="1f3c8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f3c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f3c8-128">Request body</span></span>

<span data-ttu-id="1f3c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f3c8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f3c8-130">Response</span></span>

<span data-ttu-id="1f3c8-131">В случае успеха этот метод возвращает код отклика и объект `200 OK` [authenticationListener](../resources/authenticationlistener.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f3c8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f3c8-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="1f3c8-133">Пример 1. Get an authenticationListener by id</span><span class="sxs-lookup"><span data-stu-id="1f3c8-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="1f3c8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f3c8-134">Request</span></span>

<span data-ttu-id="1f3c8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="1f3c8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f3c8-136">Response</span></span>

<span data-ttu-id="1f3c8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-137">The following is an example of the response.</span></span>

<span data-ttu-id="1f3c8-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="1f3c8-139">Пример 2. Расширение invokeUserFlowListener для определенного authenticationListener</span><span class="sxs-lookup"><span data-stu-id="1f3c8-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="1f3c8-140">В следующем примере по id получается прослушиватель для события onSignupStart и расширяется вызываемая пользовательопоток.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="1f3c8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f3c8-141">Request</span></span>

<span data-ttu-id="1f3c8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="1f3c8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f3c8-143">Response</span></span>

<span data-ttu-id="1f3c8-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-144">The following is an example of the response.</span></span>

<span data-ttu-id="1f3c8-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
