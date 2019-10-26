---
title: Обновление identityProvider
description: Обновление свойств в существующей identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cbbac43b7c47ee7aa160bf1e66a94e1afdb0c60
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734432"
---
# <a name="update-identityprovider"></a><span data-ttu-id="7adca-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="7adca-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7adca-104">Обновление свойств в существующем объекте [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7adca-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7adca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7adca-105">Permissions</span></span>

<span data-ttu-id="7adca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7adca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7adca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7adca-108">Permission type</span></span>      | <span data-ttu-id="7adca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7adca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7adca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7adca-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7adca-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7adca-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7adca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7adca-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7adca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7adca-113">Not supported.</span></span>|
|<span data-ttu-id="7adca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7adca-114">Application</span></span>| <span data-ttu-id="7adca-115">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7adca-115">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="7adca-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="7adca-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="7adca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7adca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7adca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7adca-118">Request headers</span></span>

|<span data-ttu-id="7adca-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7adca-119">Name</span></span>|<span data-ttu-id="7adca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7adca-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7adca-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7adca-121">Authorization</span></span>|<span data-ttu-id="7adca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7adca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7adca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7adca-124">Content-Type</span></span>|<span data-ttu-id="7adca-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7adca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7adca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7adca-127">Request body</span></span>

<span data-ttu-id="7adca-128">В тексте запроса предоставьте JSON-объект с одним или несколькими свойствами, требующими обновления.</span><span class="sxs-lookup"><span data-stu-id="7adca-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="7adca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7adca-129">Property</span></span>|<span data-ttu-id="7adca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7adca-130">Type</span></span>|<span data-ttu-id="7adca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7adca-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7adca-132">clientId</span><span class="sxs-lookup"><span data-stu-id="7adca-132">clientId</span></span>|<span data-ttu-id="7adca-133">String</span><span class="sxs-lookup"><span data-stu-id="7adca-133">String</span></span>|<span data-ttu-id="7adca-134">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="7adca-134">The client ID for the application.</span></span> <span data-ttu-id="7adca-135">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7adca-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7adca-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="7adca-136">clientSecret</span></span>|<span data-ttu-id="7adca-137">String</span><span class="sxs-lookup"><span data-stu-id="7adca-137">String</span></span>|<span data-ttu-id="7adca-138">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="7adca-138">The client secret for the application.</span></span> <span data-ttu-id="7adca-139">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7adca-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7adca-140">name</span><span class="sxs-lookup"><span data-stu-id="7adca-140">name</span></span>|<span data-ttu-id="7adca-141">String</span><span class="sxs-lookup"><span data-stu-id="7adca-141">String</span></span>|<span data-ttu-id="7adca-142">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7adca-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="7adca-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7adca-143">Response</span></span>

<span data-ttu-id="7adca-144">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7adca-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7adca-145">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="7adca-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7adca-146">Пример</span><span class="sxs-lookup"><span data-stu-id="7adca-146">Example</span></span>

<span data-ttu-id="7adca-147">В приведенном ниже примере обновляется определение объекта **identityProvider** времени существования маркера и оно устанавливается в качестве значения по умолчанию для организации.</span><span class="sxs-lookup"><span data-stu-id="7adca-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7adca-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7adca-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7adca-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7adca-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7adca-150">C#</span><span class="sxs-lookup"><span data-stu-id="7adca-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7adca-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7adca-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7adca-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7adca-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7adca-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7adca-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
