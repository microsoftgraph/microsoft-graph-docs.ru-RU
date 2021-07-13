---
title: Добавление userFlowIdentityProvider
description: Добавьте identityProvider в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3c30480e15b836a213a668e0948dcdb3436fbaf1
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401182"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="59c76-103">Добавление userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="59c76-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="59c76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c76-105">Добавьте поставщиков удостоверений в [объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="59c76-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59c76-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59c76-106">Permissions</span></span>

<span data-ttu-id="59c76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59c76-109">Permission type</span></span>      | <span data-ttu-id="59c76-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59c76-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59c76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59c76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59c76-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c76-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="59c76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59c76-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="59c76-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c76-114">Not supported.</span></span>|
|<span data-ttu-id="59c76-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="59c76-115">Application</span></span>| <span data-ttu-id="59c76-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c76-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="59c76-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="59c76-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="59c76-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="59c76-118">Global administrator</span></span>
* <span data-ttu-id="59c76-119">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="59c76-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="59c76-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59c76-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="59c76-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59c76-121">Request headers</span></span>

|<span data-ttu-id="59c76-122">Имя</span><span class="sxs-lookup"><span data-stu-id="59c76-122">Name</span></span>|<span data-ttu-id="59c76-123">Описание</span><span class="sxs-lookup"><span data-stu-id="59c76-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="59c76-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59c76-124">Authorization</span></span>|<span data-ttu-id="59c76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59c76-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59c76-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59c76-127">Content-Type</span></span>|<span data-ttu-id="59c76-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59c76-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59c76-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59c76-130">Request body</span></span>

<span data-ttu-id="59c76-131">В теле запроса предопрейте представление JSON с идентификатором, который `id` необходимо добавить. [](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="59c76-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="59c76-132">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в [ресурсе identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="59c76-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="59c76-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c76-133">Response</span></span>

<span data-ttu-id="59c76-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="59c76-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="59c76-135">В случае `4xx` неудачи возвращается ошибка с определенными сведениями об ошибке.</span><span class="sxs-lookup"><span data-stu-id="59c76-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="59c76-136">Пример</span><span class="sxs-lookup"><span data-stu-id="59c76-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="59c76-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="59c76-137">Request</span></span>

<span data-ttu-id="59c76-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59c76-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_userflowIdentityProviders"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="59c76-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c76-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
