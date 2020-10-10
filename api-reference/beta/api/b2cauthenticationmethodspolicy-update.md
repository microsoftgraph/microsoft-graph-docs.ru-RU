---
title: Обновление b2cAuthenticationMethodsPolicy
description: Обновление свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61c3bfa7d3fef328ed3c06d51f8c1db4ae552405
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406403"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="7a8f6-103">Обновление b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="7a8f6-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="7a8f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a8f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a8f6-105">Обновление свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7a8f6-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a8f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a8f6-106">Permissions</span></span>

<span data-ttu-id="7a8f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a8f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a8f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a8f6-109">Permission type</span></span>                        | <span data-ttu-id="7a8f6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a8f6-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="7a8f6-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a8f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a8f6-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7a8f6-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="7a8f6-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a8f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a8f6-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7a8f6-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="7a8f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a8f6-115">Application</span></span>                            | <span data-ttu-id="7a8f6-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7a8f6-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a8f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a8f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="7a8f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a8f6-118">Request headers</span></span>

|<span data-ttu-id="7a8f6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7a8f6-119">Name</span></span>|<span data-ttu-id="7a8f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7a8f6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a8f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a8f6-121">Authorization</span></span>|<span data-ttu-id="7a8f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a8f6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a8f6-124">Content-Type</span></span>|<span data-ttu-id="7a8f6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a8f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a8f6-127">Request body</span></span>

<span data-ttu-id="7a8f6-128">В тексте запроса предоставьте описание объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="7a8f6-129">В таблице ниже показаны свойства, требуемые при обновлении [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7a8f6-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="7a8f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a8f6-130">Property</span></span>     | <span data-ttu-id="7a8f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a8f6-131">Type</span></span>        | <span data-ttu-id="7a8f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a8f6-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a8f6-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="7a8f6-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="7a8f6-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="7a8f6-134">Boolean</span></span>|<span data-ttu-id="7a8f6-135">Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="7a8f6-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="7a8f6-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="7a8f6-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="7a8f6-137">Boolean</span></span>|<span data-ttu-id="7a8f6-138">Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-138">The tenant admin can configure local accounts using username if the user name and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="7a8f6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a8f6-139">Response</span></span>

<span data-ttu-id="7a8f6-140">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a8f6-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="7a8f6-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a8f6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a8f6-142">Request</span></span>

<span data-ttu-id="7a8f6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="7a8f6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a8f6-144">Response</span></span>

<span data-ttu-id="7a8f6-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7a8f6-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cauthenticationmethodspolicy"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
