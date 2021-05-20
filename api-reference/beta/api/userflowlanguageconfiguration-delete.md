---
title: Удаление userFlowLanguageConfiguration
description: Удаляет объект userFlowLanguageConfiguration из потока пользователей B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d750145561adefd7532e23ab6cbfc9bff8efe59
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546954"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="dd3ad-103">Удаление userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd3ad-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="dd3ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd3ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3ad-105">Удаляет объект [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) из потока [пользователей Azure AD B2C.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="dd3ad-106">**Примечание:** Нельзя удалять языки из потока [Azure Active Directory пользователя.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd3ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd3ad-107">Permissions</span></span>

<span data-ttu-id="dd3ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd3ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd3ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd3ad-110">Permission type</span></span>      | <span data-ttu-id="dd3ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd3ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd3ad-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd3ad-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="dd3ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dd3ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-115">Not supported.</span></span>|
|<span data-ttu-id="dd3ad-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd3ad-116">Application</span></span>|<span data-ttu-id="dd3ad-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd3ad-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="dd3ad-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="dd3ad-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="dd3ad-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="dd3ad-119">Global administrator</span></span>
* <span data-ttu-id="dd3ad-120">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="dd3ad-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="dd3ad-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd3ad-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd3ad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd3ad-122">Request headers</span></span>

|<span data-ttu-id="dd3ad-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dd3ad-123">Name</span></span>|<span data-ttu-id="dd3ad-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd3ad-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dd3ad-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd3ad-125">Authorization</span></span>|<span data-ttu-id="dd3ad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd3ad-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd3ad-128">Request body</span></span>

<span data-ttu-id="dd3ad-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd3ad-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd3ad-130">Response</span></span>

<span data-ttu-id="dd3ad-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dd3ad-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd3ad-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd3ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd3ad-133">Request</span></span>

<span data-ttu-id="dd3ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd3ad-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd3ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```
# <a name="c"></a>[<span data-ttu-id="dd3ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd3ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd3ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd3ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd3ad-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd3ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd3ad-139">Java</span><span class="sxs-lookup"><span data-stu-id="dd3ad-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd3ad-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd3ad-140">Response</span></span>

<span data-ttu-id="dd3ad-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
