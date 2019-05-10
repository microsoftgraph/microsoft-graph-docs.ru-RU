---
title: Обновление identityProvider
description: Обновление свойств в существующем объекте identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3831045172c7c3b6a0d116bd28f5dfc4462ec582
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613316"
---
# <a name="update-identityprovider"></a><span data-ttu-id="677a6-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="677a6-103">Update identityProvider</span></span>

<span data-ttu-id="677a6-104">Обновление свойств в существующем объекте [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="677a6-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="677a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="677a6-105">Permissions</span></span>

<span data-ttu-id="677a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="677a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="677a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="677a6-108">Permission type</span></span>      | <span data-ttu-id="677a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="677a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="677a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="677a6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="677a6-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="677a6-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="677a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="677a6-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="677a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677a6-113">Not supported.</span></span>|
|<span data-ttu-id="677a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="677a6-114">Application</span></span>|<span data-ttu-id="677a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677a6-115">Not supported.</span></span>|

<span data-ttu-id="677a6-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="677a6-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="677a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="677a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="677a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="677a6-118">Request headers</span></span>

|<span data-ttu-id="677a6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="677a6-119">Name</span></span>|<span data-ttu-id="677a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="677a6-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="677a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="677a6-121">Authorization</span></span>|<span data-ttu-id="677a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="677a6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="677a6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="677a6-124">Content-Type</span></span>|<span data-ttu-id="677a6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="677a6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="677a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="677a6-127">Request body</span></span>

<span data-ttu-id="677a6-128">В тексте запроса предоставьте JSON-объект с одним или несколькими свойствами, требующими обновления.</span><span class="sxs-lookup"><span data-stu-id="677a6-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="677a6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="677a6-129">Property</span></span>|<span data-ttu-id="677a6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="677a6-130">Type</span></span>|<span data-ttu-id="677a6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="677a6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="677a6-132">clientId</span><span class="sxs-lookup"><span data-stu-id="677a6-132">clientId</span></span>|<span data-ttu-id="677a6-133">String</span><span class="sxs-lookup"><span data-stu-id="677a6-133">String</span></span>|<span data-ttu-id="677a6-134">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="677a6-134">The client ID for the application.</span></span> <span data-ttu-id="677a6-135">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="677a6-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="677a6-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="677a6-136">clientSecret</span></span>|<span data-ttu-id="677a6-137">String</span><span class="sxs-lookup"><span data-stu-id="677a6-137">String</span></span>|<span data-ttu-id="677a6-138">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="677a6-138">The client secret for the application.</span></span> <span data-ttu-id="677a6-139">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="677a6-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="677a6-140">name</span><span class="sxs-lookup"><span data-stu-id="677a6-140">name</span></span>|<span data-ttu-id="677a6-141">String</span><span class="sxs-lookup"><span data-stu-id="677a6-141">String</span></span>|<span data-ttu-id="677a6-142">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="677a6-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="677a6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="677a6-143">Response</span></span>

<span data-ttu-id="677a6-144">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="677a6-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="677a6-145">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="677a6-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="677a6-146">Пример</span><span class="sxs-lookup"><span data-stu-id="677a6-146">Example</span></span>

<span data-ttu-id="677a6-147">В приведенном ниже примере обновляется определение объекта **identityProvider** времени существования маркера и оно устанавливается в качестве значения по умолчанию для организации.</span><span class="sxs-lookup"><span data-stu-id="677a6-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="677a6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="677a6-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="677a6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="677a6-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="677a6-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="677a6-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="677a6-151">C#</span><span class="sxs-lookup"><span data-stu-id="677a6-151">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="677a6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="677a6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-identityprovider-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
