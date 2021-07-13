---
title: Удаление userFlowIdentityProvider
description: Удаление identityProvider из b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: f3acd6b37092903050179ebc5377428cec7e2af0
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401170"
---
# <a name="delete-a-userflowidentityprovider"></a><span data-ttu-id="a668a-103">Удаление userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="a668a-103">Delete a userFlowIdentityProvider</span></span>

<span data-ttu-id="a668a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a668a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a668a-105">Удаление поставщика удостоверений из [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="a668a-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="a668a-106">Для самообслуживки зарегистрироваться потоки пользователей, значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="a668a-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a668a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a668a-107">Permissions</span></span>

<span data-ttu-id="a668a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a668a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a668a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a668a-110">Permission type</span></span>      | <span data-ttu-id="a668a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a668a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a668a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a668a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a668a-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a668a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a668a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a668a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a668a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a668a-115">Not supported.</span></span>|
|<span data-ttu-id="a668a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a668a-116">Application</span></span>| <span data-ttu-id="a668a-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a668a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a668a-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a668a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a668a-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a668a-119">Global administrator</span></span>
* <span data-ttu-id="a668a-120">Администратор потока внешних ID-пользователей</span><span class="sxs-lookup"><span data-stu-id="a668a-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a668a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a668a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a668a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a668a-122">Request headers</span></span>

|<span data-ttu-id="a668a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a668a-123">Name</span></span>|<span data-ttu-id="a668a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a668a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a668a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a668a-125">Authorization</span></span>|<span data-ttu-id="a668a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a668a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a668a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a668a-128">Request body</span></span>

<span data-ttu-id="a668a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a668a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a668a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a668a-130">Response</span></span>

<span data-ttu-id="a668a-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a668a-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="a668a-132">В случае `4xx` неудачи возвращается ошибка с определенными сведениями об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a668a-132">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="a668a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a668a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a668a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a668a-134">Request</span></span>

<span data-ttu-id="a668a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a668a-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

### <a name="response"></a><span data-ttu-id="a668a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a668a-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
