---
title: Удаление identityProvider из b2xIdentityUserFlow (обесценение)
description: Удаление identityProvider из b2xIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 94310d9c4ffa629638721fd248866ab685b8f506
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400952"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow-deprecated"></a><span data-ttu-id="f3978-104">Удаление identityProvider из b2xIdentityUserFlow (обесценение)</span><span class="sxs-lookup"><span data-stu-id="f3978-104">Delete identityProvider from b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="f3978-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3978-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="f3978-106">Удаление поставщика удостоверений из [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f3978-106">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="f3978-107">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="f3978-107">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3978-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3978-108">Permissions</span></span>

<span data-ttu-id="f3978-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3978-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3978-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3978-111">Permission type</span></span>      | <span data-ttu-id="f3978-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3978-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3978-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3978-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3978-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3978-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f3978-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3978-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f3978-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3978-116">Not supported.</span></span>|
|<span data-ttu-id="f3978-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3978-117">Application</span></span>| <span data-ttu-id="f3978-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3978-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f3978-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f3978-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f3978-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f3978-120">Global administrator</span></span>
* <span data-ttu-id="f3978-121">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="f3978-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f3978-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3978-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f3978-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3978-123">Request headers</span></span>

|<span data-ttu-id="f3978-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f3978-124">Name</span></span>|<span data-ttu-id="f3978-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f3978-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f3978-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3978-126">Authorization</span></span>|<span data-ttu-id="f3978-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3978-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3978-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3978-129">Request body</span></span>

<span data-ttu-id="f3978-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3978-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3978-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3978-131">Response</span></span>

<span data-ttu-id="f3978-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3978-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f3978-133">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="f3978-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f3978-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f3978-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3978-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3978-135">Request</span></span>

<span data-ttu-id="f3978-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3978-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="f3978-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3978-137">Response</span></span>

<span data-ttu-id="f3978-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3978-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
