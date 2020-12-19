---
title: Список прослушивателей onSignUpStart
description: Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d838d2a10049fa014638af0eb4a49fcbf17e3f6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720335"
---
# <a name="list-onsignupstart-listeners"></a><span data-ttu-id="2f4ad-103">Список прослушивателей onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="2f4ad-103">List onSignUpStart listeners</span></span>

<span data-ttu-id="2f4ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f4ad-105">Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-105">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span> <span data-ttu-id="2f4ad-106">Событие onSignUpStart поддерживает тип [invokeUserFlowListener.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="2f4ad-106">The onSignUpStart event supports the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) type.</span></span>

<span data-ttu-id="2f4ad-107">Когда [invokeUserFlowListener](../resources/invokeuserflowlistener.md) назначен событию onSignUpStart, приложение связано с пользовательским потоком, [](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) что позволяет самостоятельно зарегистрироваться в нем.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-107">When an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) is assigned to an onSignUpStart event, an application is associated with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process on it.</span></span> <span data-ttu-id="2f4ad-108">После создания события проверки подлинности для создания пользовательского потока пользователи, которые перейдут к этому приложению, смогут инициировать процесс регистрации, который создает гостевую учетную запись.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-108">Once the authentication event for invoking a user flow is created, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f4ad-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4ad-109">Permissions</span></span>

<span data-ttu-id="2f4ad-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f4ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f4ad-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4ad-112">Permission type</span></span>|<span data-ttu-id="2f4ad-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f4ad-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f4ad-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f4ad-114">Delegated (work or school account)</span></span>|<span data-ttu-id="2f4ad-115">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f4ad-115">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span></span>|
|<span data-ttu-id="2f4ad-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f4ad-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f4ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-117">Not supported.</span></span>|
|<span data-ttu-id="2f4ad-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f4ad-118">Application</span></span>|<span data-ttu-id="2f4ad-119">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f4ad-119">Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f4ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f4ad-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f4ad-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f4ad-121">Optional query parameters</span></span>

<span data-ttu-id="2f4ad-122">Этот метод поддерживает параметр запроса OData для расширения сведений `$expand` об invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-122">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="2f4ad-123">Пример см. ниже.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-123">See below for an example.</span></span> <span data-ttu-id="2f4ad-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2f4ad-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f4ad-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f4ad-125">Request headers</span></span>

|<span data-ttu-id="2f4ad-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2f4ad-126">Name</span></span>|<span data-ttu-id="2f4ad-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4ad-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2f4ad-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f4ad-128">Authorization</span></span>|<span data-ttu-id="2f4ad-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f4ad-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f4ad-131">Request body</span></span>

<span data-ttu-id="2f4ad-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f4ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4ad-133">Response</span></span>

<span data-ttu-id="2f4ad-134">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [authenticationListener](../resources/authenticationlistener.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-134">If successful, this method returns a `200 OK` response code and a collection of [authenticationListener](../resources/authenticationlistener.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f4ad-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f4ad-135">Examples</span></span>

### <a name="example-1-list-authenticationlisteners-for-the-onsignupstart-event"></a><span data-ttu-id="2f4ad-136">Пример 1. Список authenticationListeners для события onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="2f4ad-136">Example 1: List authenticationListeners for the onSignUpStart event</span></span>

#### <a name="request"></a><span data-ttu-id="2f4ad-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f4ad-137">Request</span></span>

<span data-ttu-id="2f4ad-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart
```

#### <a name="response"></a><span data-ttu-id="2f4ad-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4ad-139">Response</span></span>

<span data-ttu-id="2f4ad-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-140">The following is an example of the response.</span></span>

<span data-ttu-id="2f4ad-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authenticationListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      }
    },
    {
      "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
          "includeApplications": [
              "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      }
    }
  ]
}
```

### <a name="example-2-expand-invokeuserflowlisteners-in-authenticationlisteners-for-the-onsignupstart-event"></a><span data-ttu-id="2f4ad-142">Пример 2. Развернуть invokeUserFlowListeners в authenticationListeners для события onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="2f4ad-142">Example 2: Expand invokeUserFlowListeners in authenticationListeners for the onSignUpStart event</span></span>

<span data-ttu-id="2f4ad-143">В следующем примере перечисляются прослушиватели, определенные для события onSignupStart, и для каждого прослушиватель, расширяется поток пользователя, который вызывается.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-143">The following example lists the listeners defined for the onSignupStart event, and for each listener, expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="2f4ad-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f4ad-144">Request</span></span>

<span data-ttu-id="2f4ad-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart?$expand=microsoft.graph.invokeUserFlowListener/userFlow
```

#### <a name="response"></a><span data-ttu-id="2f4ad-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4ad-146">Response</span></span>

<span data-ttu-id="2f4ad-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-147">The following is an example of the response.</span></span>

<span data-ttu-id="2f4ad-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2f4ad-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.invokeUserFlowListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "value": [
    {
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
    },
    {
      "@odata.type": "#microsoft.graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
        "includeApplications": [
            "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List onSignUpStart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
