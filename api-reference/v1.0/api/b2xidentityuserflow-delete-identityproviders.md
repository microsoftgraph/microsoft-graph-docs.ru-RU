---
title: Удаление identityProvider из b2xIdentityUserFlow
description: Удаление identityProvider из b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: eb37182bf72d2e1609c3077df5e4c3a1df4a618e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883375"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="d8130-103">Удаление identityProvider из b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="d8130-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="d8130-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8130-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8130-105">Удаление поставщика удостоверений из [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="d8130-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="d8130-106">Для пользовательских потоков самообслуживки могут быть значения `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="d8130-106">For self-service sign-up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8130-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8130-107">Permissions</span></span>

<span data-ttu-id="d8130-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8130-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8130-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8130-110">Permission type</span></span>      | <span data-ttu-id="d8130-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8130-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8130-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8130-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8130-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8130-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d8130-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8130-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d8130-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8130-115">Not supported.</span></span>|
|<span data-ttu-id="d8130-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8130-116">Application</span></span>| <span data-ttu-id="d8130-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8130-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d8130-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d8130-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d8130-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d8130-119">Global administrator</span></span>
* <span data-ttu-id="d8130-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="d8130-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d8130-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8130-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d8130-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8130-122">Request headers</span></span>

|<span data-ttu-id="d8130-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d8130-123">Name</span></span>|<span data-ttu-id="d8130-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8130-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d8130-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8130-125">Authorization</span></span>|<span data-ttu-id="d8130-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8130-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8130-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8130-128">Request body</span></span>

<span data-ttu-id="d8130-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8130-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8130-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8130-130">Response</span></span>

<span data-ttu-id="d8130-131">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d8130-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="d8130-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d8130-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d8130-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d8130-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8130-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8130-134">Request</span></span>

<span data-ttu-id="d8130-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8130-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="d8130-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8130-136">Response</span></span>

<span data-ttu-id="d8130-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8130-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
