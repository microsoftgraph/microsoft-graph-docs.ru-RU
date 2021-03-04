---
title: Обновление проверки подлинностиListener
description: Обновление слушателя, определенного для события в конвейере проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 65e5fa8252bdb4b25c1992282f655f532f66e1f3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438430"
---
# <a name="update-authenticationlistener"></a><span data-ttu-id="f2cca-103">Обновление проверки подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="f2cca-103">Update authenticationListener</span></span>

<span data-ttu-id="f2cca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2cca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2cca-105">Обновление [проверки подлинностиListener,](../resources/authenticationlistener.md) определенного для события в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f2cca-105">Update the [authenticationListener](../resources/authenticationlistener.md) defined for an event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2cca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2cca-106">Permissions</span></span>

<span data-ttu-id="f2cca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2cca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2cca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2cca-109">Permission type</span></span>|<span data-ttu-id="f2cca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2cca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2cca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2cca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2cca-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2cca-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="f2cca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2cca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2cca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2cca-114">Not supported.</span></span>|
|<span data-ttu-id="f2cca-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2cca-115">Application</span></span>|<span data-ttu-id="f2cca-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2cca-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2cca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2cca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2cca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2cca-118">Request headers</span></span>

|<span data-ttu-id="f2cca-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f2cca-119">Name</span></span>|<span data-ttu-id="f2cca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2cca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2cca-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2cca-121">Authorization</span></span>|<span data-ttu-id="f2cca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2cca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f2cca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2cca-124">Content-Type</span></span>|<span data-ttu-id="f2cca-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2cca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2cca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2cca-127">Request body</span></span>

<span data-ttu-id="f2cca-128">В теле запроса поставляем представление JSON объекта [authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="f2cca-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="f2cca-129">В следующей таблице показаны свойства, необходимые при обновлении [invokeUserFlowAction.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="f2cca-129">The following table shows the properties that are required when you update the [invokeUserFlowAction](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="f2cca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2cca-130">Property</span></span>|<span data-ttu-id="f2cca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f2cca-131">Type</span></span>|<span data-ttu-id="f2cca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f2cca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2cca-133">priority</span><span class="sxs-lookup"><span data-stu-id="f2cca-133">priority</span></span>|<span data-ttu-id="f2cca-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cca-134">Int32</span></span>|<span data-ttu-id="f2cca-135">Приоритет слушателя.</span><span class="sxs-lookup"><span data-stu-id="f2cca-135">The priority of the listener.</span></span> <span data-ttu-id="f2cca-136">Определяет порядок оценки, когда в событии имеется несколько слушателей.</span><span class="sxs-lookup"><span data-stu-id="f2cca-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="f2cca-137">Приоритет оценивается от низкого до высокого.</span><span class="sxs-lookup"><span data-stu-id="f2cca-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="f2cca-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="f2cca-138">sourceFilter</span></span>|[<span data-ttu-id="f2cca-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="f2cca-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="f2cca-140">Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого.</span><span class="sxs-lookup"><span data-stu-id="f2cca-140">Filter based on the source of the authentication which is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="f2cca-141">В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="f2cca-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="response"></a><span data-ttu-id="f2cca-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2cca-142">Response</span></span>

<span data-ttu-id="f2cca-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2cca-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2cca-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2cca-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2cca-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2cca-145">Request</span></span>

<span data-ttu-id="f2cca-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2cca-146">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="f2cca-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2cca-147">Response</span></span>

<span data-ttu-id="f2cca-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2cca-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
