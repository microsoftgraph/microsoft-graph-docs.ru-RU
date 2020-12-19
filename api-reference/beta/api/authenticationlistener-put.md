---
title: Put authenticationListener
description: Замена объекта authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b5d0cfec80a04a572f3d010830423240c45a62c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720329"
---
# <a name="put-authenticationlistener"></a><span data-ttu-id="52b66-103">Put authenticationListener</span><span class="sxs-lookup"><span data-stu-id="52b66-103">Put authenticationListener</span></span>

<span data-ttu-id="52b66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b66-105">Замените [authenticationListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="52b66-105">Replace an [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="52b66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52b66-106">Permissions</span></span>

<span data-ttu-id="52b66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52b66-109">Permission type</span></span>|<span data-ttu-id="52b66-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52b66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52b66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52b66-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="52b66-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="52b66-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52b66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b66-114">Not supported.</span></span>|
|<span data-ttu-id="52b66-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="52b66-115">Application</span></span>|<span data-ttu-id="52b66-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="52b66-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="52b66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52b66-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="52b66-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52b66-118">Request headers</span></span>

|<span data-ttu-id="52b66-119">Имя</span><span class="sxs-lookup"><span data-stu-id="52b66-119">Name</span></span>|<span data-ttu-id="52b66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="52b66-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52b66-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52b66-121">Authorization</span></span>|<span data-ttu-id="52b66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b66-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="52b66-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52b66-124">Content-Type</span></span>|<span data-ttu-id="52b66-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b66-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b66-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52b66-127">Request body</span></span>

<span data-ttu-id="52b66-128">В теле запроса укажу представление объекта [authenticationListener](../resources/authenticationlistener.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="52b66-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="52b66-129">В следующей таблице показаны свойства, необходимые при создании [invokeUserFlowListener.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="52b66-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="52b66-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52b66-130">Property</span></span>|<span data-ttu-id="52b66-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52b66-131">Type</span></span>|<span data-ttu-id="52b66-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52b66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b66-133">priority</span><span class="sxs-lookup"><span data-stu-id="52b66-133">priority</span></span>|<span data-ttu-id="52b66-134">Int32</span><span class="sxs-lookup"><span data-stu-id="52b66-134">Int32</span></span>|<span data-ttu-id="52b66-135">Приоритет прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="52b66-135">The priority of the listener.</span></span> <span data-ttu-id="52b66-136">Определяет порядок оценки, если событие имеет несколько прослушивателей.</span><span class="sxs-lookup"><span data-stu-id="52b66-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="52b66-137">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="52b66-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="52b66-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="52b66-138">sourceFilter</span></span>|[<span data-ttu-id="52b66-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="52b66-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="52b66-140">Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="52b66-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="52b66-141">В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="52b66-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="52b66-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="52b66-142">userFlow</span></span>|[<span data-ttu-id="52b66-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="52b66-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="52b66-144">Ссылка на объект пользовательского потока, вызываемого в этом действии.</span><span class="sxs-lookup"><span data-stu-id="52b66-144">The reference to the user flow object that is invoked in this action.</span></span>|

## <a name="response"></a><span data-ttu-id="52b66-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b66-145">Response</span></span>

<span data-ttu-id="52b66-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52b66-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="52b66-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="52b66-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52b66-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b66-148">Request</span></span>

<span data-ttu-id="52b66-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b66-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_authenticationlistener_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
    "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
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

### <a name="response"></a><span data-ttu-id="52b66-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b66-150">Response</span></span>

<span data-ttu-id="52b66-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="52b66-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
