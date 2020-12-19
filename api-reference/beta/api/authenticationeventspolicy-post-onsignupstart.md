---
title: Создание authenticationListener
description: Создайте новый объект authenticationListener для события onSignUpStart.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5d370832032c1f80fbab31ff739706e682732f5
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720304"
---
# <a name="create-authenticationlistener"></a><span data-ttu-id="0532c-103">Создание authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0532c-103">Create authenticationListener</span></span>

<span data-ttu-id="0532c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0532c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0532c-105">Создайте новый объект authenticationListener для события onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="0532c-105">Create a new authenticationListener object for the onSignUpStart event.</span></span>

## <a name="permissions"></a><span data-ttu-id="0532c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0532c-106">Permissions</span></span>

<span data-ttu-id="0532c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0532c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0532c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0532c-109">Permission type</span></span>|<span data-ttu-id="0532c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0532c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0532c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0532c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0532c-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0532c-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="0532c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0532c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0532c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0532c-114">Not supported.</span></span>|
|<span data-ttu-id="0532c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0532c-115">Application</span></span>|<span data-ttu-id="0532c-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0532c-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="0532c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0532c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a><span data-ttu-id="0532c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0532c-118">Request headers</span></span>

|<span data-ttu-id="0532c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0532c-119">Name</span></span>|<span data-ttu-id="0532c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0532c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0532c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0532c-121">Authorization</span></span>|<span data-ttu-id="0532c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0532c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0532c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0532c-124">Content-Type</span></span>|<span data-ttu-id="0532c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0532c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0532c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0532c-127">Request body</span></span>

<span data-ttu-id="0532c-128">В теле запроса укажу представление объекта [authenticationListener](../resources/authenticationlistener.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="0532c-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="0532c-129">В следующей таблице показаны свойства, необходимые при создании [объекта invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="0532c-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.</span></span>

|<span data-ttu-id="0532c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0532c-130">Property</span></span>|<span data-ttu-id="0532c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0532c-131">Type</span></span>|<span data-ttu-id="0532c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0532c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0532c-133">priority</span><span class="sxs-lookup"><span data-stu-id="0532c-133">priority</span></span>|<span data-ttu-id="0532c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0532c-134">Int32</span></span>|<span data-ttu-id="0532c-135">Приоритет прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="0532c-135">The priority of the listener.</span></span> <span data-ttu-id="0532c-136">Определяет порядок оценки, если событие имеет несколько прослушивателей.</span><span class="sxs-lookup"><span data-stu-id="0532c-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="0532c-137">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="0532c-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="0532c-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="0532c-138">sourceFilter</span></span>|[<span data-ttu-id="0532c-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="0532c-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="0532c-140">Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="0532c-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="0532c-141">В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="0532c-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="0532c-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="0532c-142">userFlow</span></span>|[<span data-ttu-id="0532c-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0532c-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="0532c-144">Объект [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) который будет вызываться при оценке этого действия.</span><span class="sxs-lookup"><span data-stu-id="0532c-144">The [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object that will be invoked when this action is evaluated.</span></span>|

## <a name="response"></a><span data-ttu-id="0532c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0532c-145">Response</span></span>

<span data-ttu-id="0532c-146">В случае успеха этот метод возвращает код отклика и объект `201 Created` [authenticationListener](../resources/authenticationlistener.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0532c-146">If successful, this method returns a `201 Created` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0532c-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="0532c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0532c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0532c-148">Request</span></span>

<span data-ttu-id="0532c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0532c-149">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="0532c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0532c-150">Response</span></span>

<span data-ttu-id="0532c-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0532c-151">The following is an example of the response.</span></span>

<span data-ttu-id="0532c-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0532c-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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
