---
title: Создание identityProvider
description: Создание объекта identityProvider путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.
localization_priority: Normal
ms.openlocfilehash: 66f6b9bc009f207ca0eeef096791ce2877d1e45b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857594"
---
# <a name="create-identityprovider"></a><span data-ttu-id="83586-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="83586-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83586-104">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="83586-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="83586-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83586-105">Permissions</span></span>

<span data-ttu-id="83586-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83586-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83586-108">Permission type</span></span>      | <span data-ttu-id="83586-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83586-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83586-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83586-110">Delegated (work or school account)</span></span>|<span data-ttu-id="83586-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83586-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="83586-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83586-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="83586-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83586-113">Not supported.</span></span>|
|<span data-ttu-id="83586-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83586-114">Application</span></span>|<span data-ttu-id="83586-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83586-115">Not supported.</span></span>|

<span data-ttu-id="83586-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="83586-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="83586-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83586-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="83586-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83586-118">Request headers</span></span>

|<span data-ttu-id="83586-119">Имя</span><span class="sxs-lookup"><span data-stu-id="83586-119">Name</span></span>|<span data-ttu-id="83586-120">Описание</span><span class="sxs-lookup"><span data-stu-id="83586-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="83586-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83586-121">Authorization</span></span>|<span data-ttu-id="83586-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83586-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="83586-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83586-124">Content-Type</span></span>|<span data-ttu-id="83586-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83586-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83586-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83586-127">Request body</span></span>

<span data-ttu-id="83586-128">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83586-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="83586-129">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="83586-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="83586-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="83586-130">Property</span></span>|<span data-ttu-id="83586-131">Тип</span><span class="sxs-lookup"><span data-stu-id="83586-131">Type</span></span>|<span data-ttu-id="83586-132">Описание</span><span class="sxs-lookup"><span data-stu-id="83586-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83586-133">clientId</span><span class="sxs-lookup"><span data-stu-id="83586-133">clientId</span></span>|<span data-ttu-id="83586-134">String</span><span class="sxs-lookup"><span data-stu-id="83586-134">String</span></span>|<span data-ttu-id="83586-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="83586-135">The client ID for the application.</span></span> <span data-ttu-id="83586-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="83586-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="83586-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="83586-137">clientSecret</span></span>|<span data-ttu-id="83586-138">String</span><span class="sxs-lookup"><span data-stu-id="83586-138">String</span></span>|<span data-ttu-id="83586-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="83586-139">The client secret for the application.</span></span> <span data-ttu-id="83586-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="83586-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="83586-141">name</span><span class="sxs-lookup"><span data-stu-id="83586-141">name</span></span>|<span data-ttu-id="83586-142">String</span><span class="sxs-lookup"><span data-stu-id="83586-142">String</span></span>|<span data-ttu-id="83586-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="83586-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="83586-144">type</span><span class="sxs-lookup"><span data-stu-id="83586-144">type</span></span>|<span data-ttu-id="83586-145">String</span><span class="sxs-lookup"><span data-stu-id="83586-145">String</span></span>|<span data-ttu-id="83586-146">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="83586-146">The identity provider type.</span></span> <span data-ttu-id="83586-147">Он должен иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="83586-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="83586-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="83586-148">Microsoft</span></span><li/><span data-ttu-id="83586-149">Google</span><span class="sxs-lookup"><span data-stu-id="83586-149">Google</span></span><li/><span data-ttu-id="83586-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="83586-150">Amazon</span></span><li/><span data-ttu-id="83586-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="83586-151">LinkedIn</span></span><li/><span data-ttu-id="83586-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="83586-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="83586-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="83586-153">Response</span></span>

<span data-ttu-id="83586-154">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83586-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="83586-155">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="83586-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="83586-156">Пример</span><span class="sxs-lookup"><span data-stu-id="83586-156">Example</span></span>

<span data-ttu-id="83586-157">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="83586-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="83586-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="83586-158">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83586-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="83586-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="83586-160">C#</span><span class="sxs-lookup"><span data-stu-id="83586-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83586-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="83586-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83586-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="83586-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83586-163">Java</span><span class="sxs-lookup"><span data-stu-id="83586-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83586-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="83586-164">Response</span></span>

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
