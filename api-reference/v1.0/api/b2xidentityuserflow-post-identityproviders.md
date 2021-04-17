---
title: Добавление identityProvider
description: Добавление поставщика удостоверений в пользовательский поток B2X.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9ceefc258d5042877f524c5e882ea8adbdd93180
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883127"
---
# <a name="add-identityprovider"></a><span data-ttu-id="c73f3-103">Добавление identityProvider</span><span class="sxs-lookup"><span data-stu-id="c73f3-103">Add identityProvider</span></span>

<span data-ttu-id="c73f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c73f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c73f3-105">Обновление поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="c73f3-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c73f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c73f3-106">Permissions</span></span>

<span data-ttu-id="c73f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c73f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c73f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c73f3-109">Permission type</span></span>      | <span data-ttu-id="c73f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c73f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c73f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c73f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c73f3-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c73f3-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c73f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c73f3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c73f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c73f3-114">Not supported.</span></span>|
|<span data-ttu-id="c73f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c73f3-115">Application</span></span>| <span data-ttu-id="c73f3-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c73f3-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c73f3-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c73f3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c73f3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c73f3-118">Global administrator</span></span>
* <span data-ttu-id="c73f3-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="c73f3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c73f3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c73f3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c73f3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c73f3-121">Request headers</span></span>

|<span data-ttu-id="c73f3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c73f3-122">Name</span></span>|<span data-ttu-id="c73f3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c73f3-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c73f3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c73f3-124">Authorization</span></span>|<span data-ttu-id="c73f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c73f3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c73f3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c73f3-127">Content-Type</span></span>|<span data-ttu-id="c73f3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c73f3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c73f3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c73f3-130">Request body</span></span>

<span data-ttu-id="c73f3-131">В теле запроса предопрейте JSON представление `id` [идентификатораProvider,](../resources/identityprovider.md) который необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="c73f3-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="c73f3-132">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="c73f3-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="c73f3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c73f3-133">Response</span></span>

<span data-ttu-id="c73f3-134">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c73f3-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="c73f3-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="c73f3-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c73f3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c73f3-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c73f3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c73f3-137">Request</span></span>

<span data-ttu-id="c73f3-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c73f3-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"
}
```

### <a name="response"></a><span data-ttu-id="c73f3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c73f3-139">Response</span></span>

<span data-ttu-id="c73f3-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c73f3-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
