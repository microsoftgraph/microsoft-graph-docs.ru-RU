---
title: Обновление identityProvider
description: Обновление свойств в существующий identityProvider.
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077509"
---
# <a name="update-identityprovider"></a><span data-ttu-id="24d30-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="24d30-103">Update identityProvider</span></span>

> <span data-ttu-id="24d30-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24d30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24d30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24d30-106">Обновление свойств в существующий [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="24d30-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24d30-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24d30-107">Permissions</span></span>

<span data-ttu-id="24d30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24d30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24d30-110">Permission type</span></span>      | <span data-ttu-id="24d30-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24d30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24d30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24d30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24d30-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d30-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="24d30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24d30-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="24d30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d30-115">Not supported.</span></span>|
|<span data-ttu-id="24d30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24d30-116">Application</span></span>|<span data-ttu-id="24d30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d30-117">Not supported.</span></span>|

<span data-ttu-id="24d30-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="24d30-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="24d30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24d30-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="24d30-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24d30-120">Request headers</span></span>

|<span data-ttu-id="24d30-121">Имя</span><span class="sxs-lookup"><span data-stu-id="24d30-121">Name</span></span>|<span data-ttu-id="24d30-122">Описание</span><span class="sxs-lookup"><span data-stu-id="24d30-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="24d30-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24d30-123">Authorization</span></span>|<span data-ttu-id="24d30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24d30-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24d30-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24d30-126">Content-Type</span></span>|<span data-ttu-id="24d30-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24d30-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d30-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24d30-129">Request body</span></span>

<span data-ttu-id="24d30-130">Предоставить объект JSON в тексте запроса одно или несколько свойств, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="24d30-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="24d30-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="24d30-131">Property</span></span>|<span data-ttu-id="24d30-132">Тип</span><span class="sxs-lookup"><span data-stu-id="24d30-132">Type</span></span>|<span data-ttu-id="24d30-133">Description</span><span class="sxs-lookup"><span data-stu-id="24d30-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24d30-134">clientId</span><span class="sxs-lookup"><span data-stu-id="24d30-134">clientId</span></span>|<span data-ttu-id="24d30-135">String</span><span class="sxs-lookup"><span data-stu-id="24d30-135">String</span></span>|<span data-ttu-id="24d30-136">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="24d30-136">The client ID for the application.</span></span> <span data-ttu-id="24d30-137">Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="24d30-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="24d30-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="24d30-138">clientSecret</span></span>|<span data-ttu-id="24d30-139">String</span><span class="sxs-lookup"><span data-stu-id="24d30-139">String</span></span>|<span data-ttu-id="24d30-140">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="24d30-140">The client secret for the application.</span></span> <span data-ttu-id="24d30-141">Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="24d30-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="24d30-142">name</span><span class="sxs-lookup"><span data-stu-id="24d30-142">name</span></span>|<span data-ttu-id="24d30-143">String</span><span class="sxs-lookup"><span data-stu-id="24d30-143">String</span></span>|<span data-ttu-id="24d30-144">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="24d30-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="24d30-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="24d30-145">Response</span></span>

<span data-ttu-id="24d30-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24d30-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="24d30-147">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="24d30-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="24d30-148">Пример</span><span class="sxs-lookup"><span data-stu-id="24d30-148">Example</span></span>

<span data-ttu-id="24d30-149">В следующем примере происходит обновление определения срока жизни маркера **identityProvider** и устанавливает ее в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="24d30-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="24d30-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="24d30-150">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="24d30-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="24d30-151">Response</span></span>

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
  "tocPath": ""
}-->