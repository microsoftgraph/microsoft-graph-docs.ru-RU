---
title: Список доступныхProviderTypes
description: Извлечение всех доступных типов поставщика удостоверений в каталоге.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 07f18a6956fb0572168220d6cd4a28089a19430d
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491108"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="b04f7-103">Список доступныхProviderTypes</span><span class="sxs-lookup"><span data-stu-id="b04f7-103">List availableProviderTypes</span></span>

<span data-ttu-id="b04f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b04f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b04f7-105">Извлекает все типы поставщиков удостоверений, доступные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b04f7-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="b04f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b04f7-106">Permissions</span></span>

<span data-ttu-id="b04f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b04f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b04f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b04f7-109">Permission type</span></span>      | <span data-ttu-id="b04f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b04f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b04f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b04f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b04f7-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04f7-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b04f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b04f7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b04f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04f7-114">Not supported.</span></span>|
|<span data-ttu-id="b04f7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b04f7-115">Application</span></span>|<span data-ttu-id="b04f7-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04f7-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b04f7-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="b04f7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b04f7-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b04f7-118">Global Administrator</span></span>
* <span data-ttu-id="b04f7-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="b04f7-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b04f7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b04f7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="b04f7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b04f7-121">Request headers</span></span>

|<span data-ttu-id="b04f7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b04f7-122">Name</span></span>|<span data-ttu-id="b04f7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b04f7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b04f7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b04f7-124">Authorization</span></span>|<span data-ttu-id="b04f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b04f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b04f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b04f7-127">Request body</span></span>
<span data-ttu-id="b04f7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b04f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b04f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b04f7-129">Response</span></span>

<span data-ttu-id="b04f7-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b04f7-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b04f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b04f7-131">Example</span></span>

### <a name="example-1-list-all-identityprovider-available-in-an-azure-ad-directory"></a><span data-ttu-id="b04f7-132">Пример 1. Список всех **identityProvider,** доступных в каталоге Azure AD</span><span class="sxs-lookup"><span data-stu-id="b04f7-132">Example 1: List all **identityProvider** available in an Azure AD directory</span></span>

### <a name="request"></a><span data-ttu-id="b04f7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b04f7-133">Request</span></span>
<span data-ttu-id="b04f7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b04f7-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b04f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b04f7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```

---

### <a name="response"></a><span data-ttu-id="b04f7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b04f7-136">Response</span></span>

<span data-ttu-id="b04f7-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b04f7-137">The following is an example of the response.</span></span>

<span data-ttu-id="b04f7-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b04f7-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "MicrosoftAccount",
        "EmailOTP",
        "Facebook",
        "Google"
    ]
}
```

### <a name="example-2-list-all-identityprovider-available-in-an-azure-ad-b2c-directory"></a><span data-ttu-id="b04f7-139">Пример 2. Список всех **identityProvider,** доступных в каталоге Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="b04f7-139">Example 2: List all **identityProvider** available in an Azure AD B2C directory</span></span>

### <a name="request"></a><span data-ttu-id="b04f7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b04f7-140">Request</span></span>
<span data-ttu-id="b04f7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b04f7-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b04f7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b04f7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes_b2c"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```

---

### <a name="response"></a><span data-ttu-id="b04f7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b04f7-143">Response</span></span>

<span data-ttu-id="b04f7-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b04f7-144">The following is an example of the response.</span></span>

<span data-ttu-id="b04f7-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b04f7-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
  "value": [
        "Microsoft",
        "Google",
        "Facebook",
        "Amazon",
        "LinkedIn",
        "Weibo",
        "QQ",
        "WeChat",
        "Twitter",
        "GitHub",
        "AppleManaged",
        "OpenIdConnect"
  ]
}
```
