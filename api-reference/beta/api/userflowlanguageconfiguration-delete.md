---
title: Удаление userFlowLanguageConfiguration
description: Удаляет объект userFlowLanguageConfiguration из потока пользователей B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d148db0712ffbfb9ca41ba1c62e13c90c852cbc6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444751"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="ccac6-103">Удаление userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ccac6-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="ccac6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccac6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccac6-105">Удаляет объект [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) из потока [пользователей Azure AD B2C.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ccac6-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="ccac6-106">**Примечание:** Нельзя удалять языки из потока [пользователей Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ccac6-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ccac6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccac6-107">Permissions</span></span>

<span data-ttu-id="ccac6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccac6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccac6-110">Permission type</span></span>      | <span data-ttu-id="ccac6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccac6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccac6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccac6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccac6-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccac6-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ccac6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccac6-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ccac6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccac6-115">Not supported.</span></span>|
|<span data-ttu-id="ccac6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ccac6-116">Application</span></span>|<span data-ttu-id="ccac6-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccac6-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ccac6-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ccac6-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ccac6-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ccac6-119">Global administrator</span></span>
* <span data-ttu-id="ccac6-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="ccac6-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ccac6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccac6-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ccac6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccac6-122">Request headers</span></span>

|<span data-ttu-id="ccac6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ccac6-123">Name</span></span>|<span data-ttu-id="ccac6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ccac6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ccac6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccac6-125">Authorization</span></span>|<span data-ttu-id="ccac6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccac6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccac6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccac6-128">Request body</span></span>

<span data-ttu-id="ccac6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccac6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccac6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccac6-130">Response</span></span>

<span data-ttu-id="ccac6-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ccac6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ccac6-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ccac6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccac6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccac6-133">Request</span></span>

<span data-ttu-id="ccac6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccac6-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccac6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccac6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```
# <a name="c"></a>[<span data-ttu-id="ccac6-136">C#</span><span class="sxs-lookup"><span data-stu-id="ccac6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccac6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccac6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccac6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccac6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccac6-139">Java</span><span class="sxs-lookup"><span data-stu-id="ccac6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccac6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccac6-140">Response</span></span>

<span data-ttu-id="ccac6-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ccac6-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
