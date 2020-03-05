---
title: Создание identityProvider
description: Создание объекта identityProvider путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5263d67ec225aacfcee24ff22296cf8219241e09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446480"
---
# <a name="create-identityprovider"></a><span data-ttu-id="942aa-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="942aa-103">Create identityProvider</span></span>

<span data-ttu-id="942aa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="942aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942aa-105">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="942aa-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="942aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="942aa-106">Permissions</span></span>

<span data-ttu-id="942aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="942aa-109">Permission type</span></span>      | <span data-ttu-id="942aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="942aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="942aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="942aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="942aa-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942aa-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="942aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="942aa-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="942aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="942aa-114">Not supported.</span></span>|
|<span data-ttu-id="942aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="942aa-115">Application</span></span>|<span data-ttu-id="942aa-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942aa-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="942aa-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="942aa-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="942aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="942aa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="942aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="942aa-119">Request headers</span></span>

|<span data-ttu-id="942aa-120">Имя</span><span class="sxs-lookup"><span data-stu-id="942aa-120">Name</span></span>|<span data-ttu-id="942aa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="942aa-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="942aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="942aa-122">Authorization</span></span>|<span data-ttu-id="942aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="942aa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="942aa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="942aa-125">Content-Type</span></span>|<span data-ttu-id="942aa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="942aa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="942aa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="942aa-128">Request body</span></span>

<span data-ttu-id="942aa-129">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="942aa-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="942aa-130">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="942aa-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="942aa-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="942aa-131">Property</span></span>|<span data-ttu-id="942aa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="942aa-132">Type</span></span>|<span data-ttu-id="942aa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="942aa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="942aa-134">clientId</span><span class="sxs-lookup"><span data-stu-id="942aa-134">clientId</span></span>|<span data-ttu-id="942aa-135">String</span><span class="sxs-lookup"><span data-stu-id="942aa-135">String</span></span>|<span data-ttu-id="942aa-136">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="942aa-136">The client ID for the application.</span></span> <span data-ttu-id="942aa-137">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="942aa-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="942aa-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="942aa-138">clientSecret</span></span>|<span data-ttu-id="942aa-139">String</span><span class="sxs-lookup"><span data-stu-id="942aa-139">String</span></span>|<span data-ttu-id="942aa-140">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="942aa-140">The client secret for the application.</span></span> <span data-ttu-id="942aa-141">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="942aa-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="942aa-142">name</span><span class="sxs-lookup"><span data-stu-id="942aa-142">name</span></span>|<span data-ttu-id="942aa-143">String</span><span class="sxs-lookup"><span data-stu-id="942aa-143">String</span></span>|<span data-ttu-id="942aa-144">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="942aa-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="942aa-145">type</span><span class="sxs-lookup"><span data-stu-id="942aa-145">type</span></span>|<span data-ttu-id="942aa-146">String</span><span class="sxs-lookup"><span data-stu-id="942aa-146">String</span></span>|<span data-ttu-id="942aa-147">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="942aa-147">The identity provider type.</span></span> <span data-ttu-id="942aa-148">Он должен иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="942aa-148">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="942aa-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="942aa-149">Microsoft</span></span><li/><span data-ttu-id="942aa-150">Google</span><span class="sxs-lookup"><span data-stu-id="942aa-150">Google</span></span><li/><span data-ttu-id="942aa-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="942aa-151">Amazon</span></span><li/><span data-ttu-id="942aa-152">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="942aa-152">LinkedIn</span></span><li/><span data-ttu-id="942aa-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="942aa-153">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="942aa-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="942aa-154">Response</span></span>

<span data-ttu-id="942aa-155">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="942aa-155">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="942aa-156">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="942aa-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="942aa-157">Пример</span><span class="sxs-lookup"><span data-stu-id="942aa-157">Example</span></span>

<span data-ttu-id="942aa-158">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="942aa-158">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="942aa-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="942aa-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="942aa-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="942aa-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="942aa-161">C#</span><span class="sxs-lookup"><span data-stu-id="942aa-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="942aa-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="942aa-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="942aa-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="942aa-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="942aa-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="942aa-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
