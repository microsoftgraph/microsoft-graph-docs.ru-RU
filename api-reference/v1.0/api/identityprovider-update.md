---
title: Обновление identityProvider
description: Обновление свойств в существующем объекте identityProvider
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 023797466cc1574343a64776ecb0dcaf226be04c
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199889"
---
# <a name="update-identityprovider"></a><span data-ttu-id="4c151-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="4c151-103">Update identityProvider</span></span>

<span data-ttu-id="4c151-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c151-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c151-105">Обновление свойств в существующем объекте [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4c151-105">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c151-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c151-106">Permissions</span></span>

<span data-ttu-id="4c151-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c151-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c151-109">Permission type</span></span>      | <span data-ttu-id="4c151-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c151-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c151-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c151-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c151-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c151-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4c151-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c151-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4c151-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c151-114">Not supported.</span></span>|
|<span data-ttu-id="4c151-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c151-115">Application</span></span>|<span data-ttu-id="4c151-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c151-116">Not supported.</span></span>|

<span data-ttu-id="4c151-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="4c151-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4c151-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c151-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c151-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c151-119">Request headers</span></span>

|<span data-ttu-id="4c151-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4c151-120">Name</span></span>|<span data-ttu-id="4c151-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4c151-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4c151-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c151-122">Authorization</span></span>|<span data-ttu-id="4c151-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c151-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c151-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c151-125">Content-Type</span></span>|<span data-ttu-id="4c151-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c151-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c151-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c151-128">Request body</span></span>

<span data-ttu-id="4c151-129">В тексте запроса предоставьте JSON-объект с одним или несколькими свойствами, требующими обновления.</span><span class="sxs-lookup"><span data-stu-id="4c151-129">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="4c151-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c151-130">Property</span></span>|<span data-ttu-id="4c151-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c151-131">Type</span></span>|<span data-ttu-id="4c151-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c151-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c151-133">clientId</span><span class="sxs-lookup"><span data-stu-id="4c151-133">clientId</span></span>|<span data-ttu-id="4c151-134">String</span><span class="sxs-lookup"><span data-stu-id="4c151-134">String</span></span>|<span data-ttu-id="4c151-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c151-135">The client ID for the application.</span></span> <span data-ttu-id="4c151-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c151-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c151-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="4c151-137">clientSecret</span></span>|<span data-ttu-id="4c151-138">String</span><span class="sxs-lookup"><span data-stu-id="4c151-138">String</span></span>|<span data-ttu-id="4c151-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c151-139">The client secret for the application.</span></span> <span data-ttu-id="4c151-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c151-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c151-141">name</span><span class="sxs-lookup"><span data-stu-id="4c151-141">name</span></span>|<span data-ttu-id="4c151-142">String</span><span class="sxs-lookup"><span data-stu-id="4c151-142">String</span></span>|<span data-ttu-id="4c151-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c151-143">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="4c151-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c151-144">Response</span></span>

<span data-ttu-id="4c151-145">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c151-145">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="4c151-146">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="4c151-146">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="4c151-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4c151-147">Example</span></span>

<span data-ttu-id="4c151-148">В приведенном ниже примере обновляется определение объекта **identityProvider** времени существования маркера и оно устанавливается в качестве значения по умолчанию для организации.</span><span class="sxs-lookup"><span data-stu-id="4c151-148">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="4c151-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c151-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4c151-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c151-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[<span data-ttu-id="4c151-151">C#</span><span class="sxs-lookup"><span data-stu-id="4c151-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c151-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c151-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c151-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c151-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c151-154">Java</span><span class="sxs-lookup"><span data-stu-id="4c151-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c151-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c151-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
