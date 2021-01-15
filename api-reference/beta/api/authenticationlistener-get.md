---
title: Get authenticationListener
description: Чтение свойств и связей объекта authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3e6f07ac59e143ab7e9723c5a5b81a4c8489e54
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872424"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="804bc-103">Get authenticationListener</span><span class="sxs-lookup"><span data-stu-id="804bc-103">Get authenticationListener</span></span>

<span data-ttu-id="804bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="804bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804bc-105">Получите указанный [authenticationListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="804bc-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="804bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="804bc-106">Permissions</span></span>

<span data-ttu-id="804bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="804bc-109">Permission type</span></span>|<span data-ttu-id="804bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="804bc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="804bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="804bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="804bc-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="804bc-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="804bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="804bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="804bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="804bc-114">Not supported.</span></span>|
|<span data-ttu-id="804bc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="804bc-115">Application</span></span>|<span data-ttu-id="804bc-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="804bc-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="804bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="804bc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="804bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="804bc-118">Optional query parameters</span></span>

<span data-ttu-id="804bc-119">Этот метод поддерживает параметр запроса OData для расширения сведений `$expand` об invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="804bc-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="804bc-120">См. пример ниже.</span><span class="sxs-lookup"><span data-stu-id="804bc-120">See below for an example.</span></span> <span data-ttu-id="804bc-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="804bc-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="804bc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="804bc-122">Request headers</span></span>

|<span data-ttu-id="804bc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="804bc-123">Name</span></span>|<span data-ttu-id="804bc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="804bc-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="804bc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="804bc-125">Authorization</span></span>|<span data-ttu-id="804bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="804bc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="804bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="804bc-128">Request body</span></span>

<span data-ttu-id="804bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="804bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="804bc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="804bc-130">Response</span></span>

<span data-ttu-id="804bc-131">В случае успеха этот метод возвращает код отклика и объект `200 OK` [authenticationListener](../resources/authenticationlistener.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="804bc-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="804bc-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="804bc-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="804bc-133">Пример 1. Get an authenticationListener by id</span><span class="sxs-lookup"><span data-stu-id="804bc-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="804bc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="804bc-134">Request</span></span>

<span data-ttu-id="804bc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="804bc-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="804bc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="804bc-136">Response</span></span>

<span data-ttu-id="804bc-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="804bc-137">The following is an example of the response.</span></span>

<span data-ttu-id="804bc-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="804bc-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="804bc-139">Пример 2. Расширение invokeUserFlowListener для определенного authenticationListener</span><span class="sxs-lookup"><span data-stu-id="804bc-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="804bc-140">В следующем примере по id получается прослушиватель для события onSignupStart и расширяется вызываемая пользовательопоток.</span><span class="sxs-lookup"><span data-stu-id="804bc-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="804bc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="804bc-141">Request</span></span>

<span data-ttu-id="804bc-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="804bc-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="804bc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="804bc-143">Response</span></span>

<span data-ttu-id="804bc-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="804bc-144">The following is an example of the response.</span></span>

<span data-ttu-id="804bc-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="804bc-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
