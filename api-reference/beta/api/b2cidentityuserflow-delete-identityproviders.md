---
title: Удаление identityProvider из b2cIdentityUserFlow (обесценение)
description: Удаление identityProvider из b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: a6d825cd474a38176256e0e18dd6b77d1345a64b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400994"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="c060c-104">Удаление идентификатораProvider из b2cIdentityUserFlow (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="c060c-104">Delete an identityProvider from a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="c060c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c060c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="c060c-106">Удаление поставщика удостоверений из [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="c060c-106">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="c060c-107">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="c060c-107">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="c060c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c060c-108">Permissions</span></span>

<span data-ttu-id="c060c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c060c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c060c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c060c-111">Permission type</span></span>      | <span data-ttu-id="c060c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c060c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c060c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c060c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c060c-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c060c-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c060c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c060c-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c060c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c060c-116">Not supported.</span></span>|
|<span data-ttu-id="c060c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c060c-117">Application</span></span>| <span data-ttu-id="c060c-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c060c-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c060c-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c060c-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c060c-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c060c-120">Global administrator</span></span>
* <span data-ttu-id="c060c-121">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="c060c-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c060c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c060c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c060c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c060c-123">Request headers</span></span>

|<span data-ttu-id="c060c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c060c-124">Name</span></span>|<span data-ttu-id="c060c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c060c-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c060c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c060c-126">Authorization</span></span>|<span data-ttu-id="c060c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c060c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c060c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c060c-129">Request body</span></span>

<span data-ttu-id="c060c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c060c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c060c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c060c-131">Response</span></span>

<span data-ttu-id="c060c-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c060c-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="c060c-133">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="c060c-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c060c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c060c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c060c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c060c-135">Request</span></span>

<span data-ttu-id="c060c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c060c-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="c060c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c060c-137">Response</span></span>

<span data-ttu-id="c060c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c060c-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
