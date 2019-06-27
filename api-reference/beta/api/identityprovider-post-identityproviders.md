---
title: Создание identityProvider
description: Создание объекта identityProvider путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.
localization_priority: Normal
ms.openlocfilehash: 97a87d73090457a2e314a8b44903260b24e55a69
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262673"
---
# <a name="create-identityprovider"></a><span data-ttu-id="62950-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="62950-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62950-104">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="62950-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="62950-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62950-105">Permissions</span></span>

<span data-ttu-id="62950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62950-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62950-108">Permission type</span></span>      | <span data-ttu-id="62950-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62950-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62950-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62950-110">Delegated (work or school account)</span></span>|<span data-ttu-id="62950-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62950-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="62950-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62950-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="62950-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62950-113">Not supported.</span></span>|
|<span data-ttu-id="62950-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62950-114">Application</span></span>|<span data-ttu-id="62950-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62950-115">Not supported.</span></span>|

<span data-ttu-id="62950-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="62950-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="62950-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62950-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="62950-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62950-118">Request headers</span></span>

|<span data-ttu-id="62950-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62950-119">Name</span></span>|<span data-ttu-id="62950-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62950-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="62950-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62950-121">Authorization</span></span>|<span data-ttu-id="62950-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62950-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62950-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62950-124">Content-Type</span></span>|<span data-ttu-id="62950-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62950-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62950-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62950-127">Request body</span></span>

<span data-ttu-id="62950-128">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62950-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="62950-129">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="62950-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="62950-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62950-130">Property</span></span>|<span data-ttu-id="62950-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62950-131">Type</span></span>|<span data-ttu-id="62950-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62950-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62950-133">clientId</span><span class="sxs-lookup"><span data-stu-id="62950-133">clientId</span></span>|<span data-ttu-id="62950-134">String</span><span class="sxs-lookup"><span data-stu-id="62950-134">String</span></span>|<span data-ttu-id="62950-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="62950-135">The client ID for the application.</span></span> <span data-ttu-id="62950-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="62950-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="62950-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="62950-137">clientSecret</span></span>|<span data-ttu-id="62950-138">String</span><span class="sxs-lookup"><span data-stu-id="62950-138">String</span></span>|<span data-ttu-id="62950-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="62950-139">The client secret for the application.</span></span> <span data-ttu-id="62950-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="62950-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="62950-141">name</span><span class="sxs-lookup"><span data-stu-id="62950-141">name</span></span>|<span data-ttu-id="62950-142">String</span><span class="sxs-lookup"><span data-stu-id="62950-142">String</span></span>|<span data-ttu-id="62950-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="62950-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="62950-144">type</span><span class="sxs-lookup"><span data-stu-id="62950-144">type</span></span>|<span data-ttu-id="62950-145">String</span><span class="sxs-lookup"><span data-stu-id="62950-145">String</span></span>|<span data-ttu-id="62950-146">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="62950-146">The identity provider type.</span></span> <span data-ttu-id="62950-147">Он должен иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="62950-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="62950-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="62950-148">Microsoft</span></span><li/><span data-ttu-id="62950-149">Google</span><span class="sxs-lookup"><span data-stu-id="62950-149">Google</span></span><li/><span data-ttu-id="62950-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="62950-150">Amazon</span></span><li/><span data-ttu-id="62950-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="62950-151">LinkedIn</span></span><li/><span data-ttu-id="62950-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="62950-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="62950-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="62950-153">Response</span></span>

<span data-ttu-id="62950-154">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62950-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="62950-155">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="62950-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="62950-156">Пример</span><span class="sxs-lookup"><span data-stu-id="62950-156">Example</span></span>

<span data-ttu-id="62950-157">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="62950-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="62950-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="62950-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="62950-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="62950-159">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="62950-160">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="62950-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62950-161">C#</span><span class="sxs-lookup"><span data-stu-id="62950-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62950-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="62950-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62950-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="62950-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
