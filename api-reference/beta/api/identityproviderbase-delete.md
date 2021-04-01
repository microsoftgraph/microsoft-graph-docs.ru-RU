---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: cdacaf4495d6856bc39465d4bed990a20cd264e7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491114"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="9fe4a-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="9fe4a-103">Delete identityProvider</span></span>
<span data-ttu-id="9fe4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fe4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fe4a-105">Удаление объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="9fe4a-106">В Azure AD B2C удалите [объект socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объект appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="9fe4a-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fe4a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fe4a-107">Permissions</span></span>

<span data-ttu-id="9fe4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fe4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe4a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fe4a-110">Permission type</span></span>      | <span data-ttu-id="9fe4a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fe4a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fe4a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fe4a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fe4a-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe4a-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9fe4a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fe4a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9fe4a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-115">Not supported.</span></span>|
|<span data-ttu-id="9fe4a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9fe4a-116">Application</span></span>|<span data-ttu-id="9fe4a-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe4a-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="9fe4a-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="9fe4a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9fe4a-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9fe4a-119">Global Administrator</span></span>
* <span data-ttu-id="9fe4a-120">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="9fe4a-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9fe4a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fe4a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9fe4a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fe4a-122">Request headers</span></span>

|<span data-ttu-id="9fe4a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9fe4a-123">Name</span></span>|<span data-ttu-id="9fe4a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe4a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9fe4a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fe4a-125">Authorization</span></span>|<span data-ttu-id="9fe4a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fe4a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fe4a-128">Request body</span></span>

<span data-ttu-id="9fe4a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fe4a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fe4a-130">Response</span></span>

<span data-ttu-id="9fe4a-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9fe4a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9fe4a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fe4a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fe4a-133">Request</span></span>

<span data-ttu-id="9fe4a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-134">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```

### <a name="response"></a><span data-ttu-id="9fe4a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fe4a-135">Response</span></span>

<span data-ttu-id="9fe4a-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-136">The following is an example of the response.</span></span>

<span data-ttu-id="9fe4a-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9fe4a-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
