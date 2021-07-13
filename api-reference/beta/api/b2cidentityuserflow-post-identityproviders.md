---
title: Добавление identityProvider в b2cIdentityUserFlow (обесценение)
description: Добавьте identityProvider в b2cIdentityUserFlow. (неоконт.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9b213dd0255984b0ffe99270ec5fa7f69558aabb
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400966"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="2f93d-104">Добавление identityProvider в b2cIdentityUserFlow (обесценение)</span><span class="sxs-lookup"><span data-stu-id="2f93d-104">Add identityProvider to a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="2f93d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f93d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="2f93d-106">Добавление поставщиков удостоверений в [объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="2f93d-106">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f93d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f93d-107">Permissions</span></span>

<span data-ttu-id="2f93d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f93d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f93d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f93d-110">Permission type</span></span>      | <span data-ttu-id="2f93d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f93d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f93d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f93d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f93d-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f93d-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2f93d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f93d-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2f93d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f93d-115">Not supported.</span></span>|
|<span data-ttu-id="2f93d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f93d-116">Application</span></span>| <span data-ttu-id="2f93d-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f93d-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2f93d-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="2f93d-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2f93d-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2f93d-119">Global administrator</span></span>
* <span data-ttu-id="2f93d-120">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="2f93d-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2f93d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f93d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2f93d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f93d-122">Request headers</span></span>

|<span data-ttu-id="2f93d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2f93d-123">Name</span></span>|<span data-ttu-id="2f93d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2f93d-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2f93d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f93d-125">Authorization</span></span>|<span data-ttu-id="2f93d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f93d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2f93d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f93d-128">Content-Type</span></span>|<span data-ttu-id="2f93d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f93d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f93d-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f93d-131">Request body</span></span>

<span data-ttu-id="2f93d-132">В теле запроса предопрейте JSON представление `id` [идентификатораProvider,](../resources/identityprovider.md) который необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="2f93d-132">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="2f93d-133">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="2f93d-133">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="2f93d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f93d-134">Response</span></span>

<span data-ttu-id="2f93d-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2f93d-135">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="2f93d-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="2f93d-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2f93d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="2f93d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f93d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f93d-138">Request</span></span>

<span data-ttu-id="2f93d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f93d-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="2f93d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f93d-140">Response</span></span>

<span data-ttu-id="2f93d-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f93d-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
