---
title: Создание identityProvider
description: Создание объекта identityProvider путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96d794670c185e8c06b0cf5c34315dbb2f2fbadc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734460"
---
# <a name="create-identityprovider"></a><span data-ttu-id="fe4bd-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="fe4bd-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe4bd-104">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe4bd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe4bd-105">Permissions</span></span>

<span data-ttu-id="fe4bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe4bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe4bd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe4bd-108">Permission type</span></span>      | <span data-ttu-id="fe4bd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe4bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe4bd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe4bd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="fe4bd-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe4bd-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fe4bd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe4bd-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fe4bd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-113">Not supported.</span></span>|
|<span data-ttu-id="fe4bd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe4bd-114">Application</span></span>|<span data-ttu-id="fe4bd-115">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe4bd-115">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="fe4bd-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe4bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe4bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="fe4bd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe4bd-118">Request headers</span></span>

|<span data-ttu-id="fe4bd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fe4bd-119">Name</span></span>|<span data-ttu-id="fe4bd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fe4bd-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fe4bd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe4bd-121">Authorization</span></span>|<span data-ttu-id="fe4bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe4bd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe4bd-124">Content-Type</span></span>|<span data-ttu-id="fe4bd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe4bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe4bd-127">Request body</span></span>

<span data-ttu-id="fe4bd-128">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="fe4bd-129">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="fe4bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe4bd-130">Property</span></span>|<span data-ttu-id="fe4bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe4bd-131">Type</span></span>|<span data-ttu-id="fe4bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe4bd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe4bd-133">clientId</span><span class="sxs-lookup"><span data-stu-id="fe4bd-133">clientId</span></span>|<span data-ttu-id="fe4bd-134">String</span><span class="sxs-lookup"><span data-stu-id="fe4bd-134">String</span></span>|<span data-ttu-id="fe4bd-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-135">The client ID for the application.</span></span> <span data-ttu-id="fe4bd-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fe4bd-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="fe4bd-137">clientSecret</span></span>|<span data-ttu-id="fe4bd-138">String</span><span class="sxs-lookup"><span data-stu-id="fe4bd-138">String</span></span>|<span data-ttu-id="fe4bd-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-139">The client secret for the application.</span></span> <span data-ttu-id="fe4bd-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fe4bd-141">name</span><span class="sxs-lookup"><span data-stu-id="fe4bd-141">name</span></span>|<span data-ttu-id="fe4bd-142">String</span><span class="sxs-lookup"><span data-stu-id="fe4bd-142">String</span></span>|<span data-ttu-id="fe4bd-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="fe4bd-144">type</span><span class="sxs-lookup"><span data-stu-id="fe4bd-144">type</span></span>|<span data-ttu-id="fe4bd-145">String</span><span class="sxs-lookup"><span data-stu-id="fe4bd-145">String</span></span>|<span data-ttu-id="fe4bd-146">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="fe4bd-146">The identity provider type.</span></span> <span data-ttu-id="fe4bd-147">Он должен иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="fe4bd-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="fe4bd-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="fe4bd-148">Microsoft</span></span><li/><span data-ttu-id="fe4bd-149">Google</span><span class="sxs-lookup"><span data-stu-id="fe4bd-149">Google</span></span><li/><span data-ttu-id="fe4bd-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="fe4bd-150">Amazon</span></span><li/><span data-ttu-id="fe4bd-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="fe4bd-151">LinkedIn</span></span><li/><span data-ttu-id="fe4bd-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="fe4bd-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="fe4bd-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe4bd-153">Response</span></span>

<span data-ttu-id="fe4bd-154">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="fe4bd-155">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="fe4bd-156">Пример</span><span class="sxs-lookup"><span data-stu-id="fe4bd-156">Example</span></span>

<span data-ttu-id="fe4bd-157">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="fe4bd-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="fe4bd-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe4bd-158">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe4bd-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe4bd-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe4bd-160">C#</span><span class="sxs-lookup"><span data-stu-id="fe4bd-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe4bd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe4bd-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe4bd-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe4bd-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe4bd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe4bd-163">Response</span></span>

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
