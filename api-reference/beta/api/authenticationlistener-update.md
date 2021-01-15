---
title: Обновление authenticationListener
description: Обновим прослушиватель, определенный для события в конвейере проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5acb660843bf0b7a60fd66886841ab4c490f396
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872396"
---
# <a name="update-authenticationlistener"></a><span data-ttu-id="50bb0-103">Обновление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="50bb0-103">Update authenticationListener</span></span>

<span data-ttu-id="50bb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50bb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50bb0-105">Обновление [authenticationListener,](../resources/authenticationlistener.md) определенного для события в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="50bb0-105">Update the [authenticationListener](../resources/authenticationlistener.md) defined for an event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="50bb0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50bb0-106">Permissions</span></span>

<span data-ttu-id="50bb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50bb0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50bb0-109">Permission type</span></span>|<span data-ttu-id="50bb0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50bb0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50bb0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50bb0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50bb0-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="50bb0-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="50bb0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50bb0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50bb0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bb0-114">Not supported.</span></span>|
|<span data-ttu-id="50bb0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="50bb0-115">Application</span></span>|<span data-ttu-id="50bb0-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="50bb0-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="50bb0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50bb0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="50bb0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50bb0-118">Request headers</span></span>

|<span data-ttu-id="50bb0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="50bb0-119">Name</span></span>|<span data-ttu-id="50bb0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="50bb0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="50bb0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50bb0-121">Authorization</span></span>|<span data-ttu-id="50bb0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50bb0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="50bb0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50bb0-124">Content-Type</span></span>|<span data-ttu-id="50bb0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50bb0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50bb0-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="50bb0-127">Request body</span></span>

<span data-ttu-id="50bb0-128">В теле запроса укажу представление объекта [authenticationListener](../resources/authenticationlistener.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="50bb0-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="50bb0-129">В следующей таблице показаны свойства, необходимые при обновлении [invokeUserFlowAction.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="50bb0-129">The following table shows the properties that are required when you update the [invokeUserFlowAction](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="50bb0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50bb0-130">Property</span></span>|<span data-ttu-id="50bb0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50bb0-131">Type</span></span>|<span data-ttu-id="50bb0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50bb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50bb0-133">priority</span><span class="sxs-lookup"><span data-stu-id="50bb0-133">priority</span></span>|<span data-ttu-id="50bb0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="50bb0-134">Int32</span></span>|<span data-ttu-id="50bb0-135">Приоритет прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="50bb0-135">The priority of the listener.</span></span> <span data-ttu-id="50bb0-136">Определяет порядок оценки, если событие имеет несколько прослушивателей.</span><span class="sxs-lookup"><span data-stu-id="50bb0-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="50bb0-137">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="50bb0-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="50bb0-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="50bb0-138">sourceFilter</span></span>|[<span data-ttu-id="50bb0-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="50bb0-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="50bb0-140">Фильтр на основе источника проверки подлинности, который используется для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="50bb0-140">Filter based on the source of the authentication which is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="50bb0-141">В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="50bb0-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="response"></a><span data-ttu-id="50bb0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bb0-142">Response</span></span>

<span data-ttu-id="50bb0-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50bb0-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="50bb0-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="50bb0-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50bb0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="50bb0-145">Request</span></span>

<span data-ttu-id="50bb0-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50bb0-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onsignupstart"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
  "priority": 101
}
```

### <a name="response"></a><span data-ttu-id="50bb0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bb0-147">Response</span></span>

<span data-ttu-id="50bb0-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="50bb0-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
