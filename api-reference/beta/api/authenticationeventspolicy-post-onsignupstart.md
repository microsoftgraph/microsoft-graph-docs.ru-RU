---
title: Создание authenticationListener
description: Создайте новый объект authenticationListener для события onSignUpStart.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c24ceff80c873181799ea38fbe23c6054f876bc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438535"
---
# <a name="create-authenticationlistener"></a><span data-ttu-id="3b930-103">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="3b930-103">Create authenticationListener</span></span>

<span data-ttu-id="3b930-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b930-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b930-105">Создайте новый объект authenticationListener для события onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="3b930-105">Create a new authenticationListener object for the onSignUpStart event.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b930-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b930-106">Permissions</span></span>

<span data-ttu-id="3b930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b930-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b930-109">Permission type</span></span>|<span data-ttu-id="3b930-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b930-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b930-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b930-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b930-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b930-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="3b930-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b930-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b930-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b930-114">Not supported.</span></span>|
|<span data-ttu-id="3b930-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b930-115">Application</span></span>|<span data-ttu-id="3b930-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b930-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b930-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b930-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a><span data-ttu-id="3b930-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b930-118">Request headers</span></span>

|<span data-ttu-id="3b930-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3b930-119">Name</span></span>|<span data-ttu-id="3b930-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b930-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b930-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b930-121">Authorization</span></span>|<span data-ttu-id="3b930-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b930-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3b930-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b930-124">Content-Type</span></span>|<span data-ttu-id="3b930-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b930-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b930-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b930-127">Request body</span></span>

<span data-ttu-id="3b930-128">В теле запроса поставляем представление JSON объекта [authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="3b930-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="3b930-129">В следующей таблице показаны свойства, необходимые при создании проверки подлинности [invokeUserFlowListener.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="3b930-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.</span></span>

|<span data-ttu-id="3b930-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b930-130">Property</span></span>|<span data-ttu-id="3b930-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b930-131">Type</span></span>|<span data-ttu-id="3b930-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b930-133">priority</span><span class="sxs-lookup"><span data-stu-id="3b930-133">priority</span></span>|<span data-ttu-id="3b930-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3b930-134">Int32</span></span>|<span data-ttu-id="3b930-135">Приоритет слушателя.</span><span class="sxs-lookup"><span data-stu-id="3b930-135">The priority of the listener.</span></span> <span data-ttu-id="3b930-136">Определяет порядок оценки, когда в событии имеется несколько слушателей.</span><span class="sxs-lookup"><span data-stu-id="3b930-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="3b930-137">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="3b930-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="3b930-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="3b930-138">sourceFilter</span></span>|[<span data-ttu-id="3b930-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="3b930-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="3b930-140">Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого.</span><span class="sxs-lookup"><span data-stu-id="3b930-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="3b930-141">В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="3b930-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="3b930-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="3b930-142">userFlow</span></span>|[<span data-ttu-id="3b930-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3b930-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="3b930-144">Объект [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) который будет вызываться при оценке этого действия.</span><span class="sxs-lookup"><span data-stu-id="3b930-144">The [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object that will be invoked when this action is evaluated.</span></span>|

## <a name="response"></a><span data-ttu-id="3b930-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b930-145">Response</span></span>

<span data-ttu-id="3b930-146">В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [authenticationListener](../resources/authenticationlistener.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b930-146">If successful, this method returns a `201 Created` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b930-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b930-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b930-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b930-148">Request</span></span>

<span data-ttu-id="3b930-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b930-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_authenticationlistener_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/events/onSignupStart
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    },
    "userFlow": {
        "id": "B2X_1_Partner"
    }
}
```

### <a name="response"></a><span data-ttu-id="3b930-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b930-150">Response</span></span>

<span data-ttu-id="3b930-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b930-151">The following is an example of the response.</span></span>

<span data-ttu-id="3b930-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b930-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/events/onSignupStart/Microsoft.Graph.InvokeUserFlowListener/$entity",
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "id": "2be3336b-e3b4-44f3-9128-b6fd9ad39bb8",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    }
}
```
