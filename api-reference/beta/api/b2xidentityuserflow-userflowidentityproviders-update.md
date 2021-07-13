---
title: Обновление userFlowIdentityProvider
description: Обновление identityProvider в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 61b5ea598b6a82c9ecacf3610792164717b4a965
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401150"
---
# <a name="update-a-userflowidentityprovider"></a><span data-ttu-id="67990-103">Обновление userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="67990-103">Update a userFlowIdentityProvider</span></span>

<span data-ttu-id="67990-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67990-105">Обновление поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="67990-105">Update an identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67990-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67990-106">Permissions</span></span>

<span data-ttu-id="67990-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67990-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67990-109">Permission type</span></span>      | <span data-ttu-id="67990-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67990-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67990-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67990-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67990-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67990-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="67990-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67990-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="67990-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67990-114">Not supported.</span></span>|
|<span data-ttu-id="67990-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="67990-115">Application</span></span>| <span data-ttu-id="67990-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67990-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="67990-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="67990-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="67990-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="67990-118">Global administrator</span></span>
* <span data-ttu-id="67990-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="67990-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="67990-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67990-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="67990-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67990-121">Request headers</span></span>

|<span data-ttu-id="67990-122">Имя</span><span class="sxs-lookup"><span data-stu-id="67990-122">Name</span></span>|<span data-ttu-id="67990-123">Описание</span><span class="sxs-lookup"><span data-stu-id="67990-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="67990-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67990-124">Authorization</span></span>|<span data-ttu-id="67990-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67990-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67990-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67990-127">Content-Type</span></span>|<span data-ttu-id="67990-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67990-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67990-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67990-130">Request body</span></span>

<span data-ttu-id="67990-131">В теле запроса предопрейте представление JSON с идентификатором, который `id` необходимо добавить. [](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="67990-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="67990-132">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="67990-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="67990-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="67990-133">Response</span></span>

<span data-ttu-id="67990-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67990-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="67990-135">В случае `4xx` неудачи возвращается ошибка с определенными сведениями об ошибке.</span><span class="sxs-lookup"><span data-stu-id="67990-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="67990-136">Пример</span><span class="sxs-lookup"><span data-stu-id="67990-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="67990-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="67990-137">Request</span></span>

<span data-ttu-id="67990-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67990-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_userflowidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"
}
```

### <a name="response"></a><span data-ttu-id="67990-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="67990-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
