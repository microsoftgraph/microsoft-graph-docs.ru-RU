---
title: Удаление userflowidentityproviders
description: Удаление identityProvider из b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4ad44addce58e8f18c0b6d582f0fd6f821cfc1c5
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401187"
---
# <a name="delete-a-userflowidentityproviders"></a><span data-ttu-id="e33d0-103">Удаление userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="e33d0-103">Delete a userflowidentityproviders</span></span>

<span data-ttu-id="e33d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e33d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e33d0-105">Удаление поставщика удостоверений из [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e33d0-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="e33d0-106">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="e33d0-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="e33d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e33d0-107">Permissions</span></span>

<span data-ttu-id="e33d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e33d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e33d0-110">Permission type</span></span>      | <span data-ttu-id="e33d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e33d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e33d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e33d0-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e33d0-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e33d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e33d0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e33d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e33d0-115">Not supported.</span></span>|
|<span data-ttu-id="e33d0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e33d0-116">Application</span></span>| <span data-ttu-id="e33d0-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e33d0-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e33d0-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e33d0-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e33d0-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e33d0-119">Global administrator</span></span>
* <span data-ttu-id="e33d0-120">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="e33d0-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e33d0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e33d0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e33d0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e33d0-122">Request headers</span></span>

|<span data-ttu-id="e33d0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e33d0-123">Name</span></span>|<span data-ttu-id="e33d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e33d0-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e33d0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e33d0-125">Authorization</span></span>|<span data-ttu-id="e33d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e33d0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33d0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e33d0-128">Request body</span></span>

<span data-ttu-id="e33d0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e33d0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e33d0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e33d0-130">Response</span></span>

<span data-ttu-id="e33d0-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e33d0-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e33d0-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="e33d0-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e33d0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e33d0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e33d0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e33d0-134">Request</span></span>

<span data-ttu-id="e33d0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e33d0-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref
```

### <a name="response"></a><span data-ttu-id="e33d0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e33d0-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
