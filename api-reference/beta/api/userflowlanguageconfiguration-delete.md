---
title: Удаление userFlowLanguageConfiguration
description: Удаляет объект userFlowLanguageConfiguration из пользовательского потока B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b9a59c8786fa27b458fd6f1236a30e33f1fb355
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844963"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="f5576-103">Удаление userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5576-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="f5576-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5576-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5576-105">Удаляет объект [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) из пользовательского потока [B2C Azure AD.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f5576-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="f5576-106">**Примечание.** Вы не можете удалить языки из пользовательского [потока Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f5576-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5576-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5576-107">Permissions</span></span>

<span data-ttu-id="f5576-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5576-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5576-110">Permission type</span></span>      | <span data-ttu-id="f5576-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5576-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5576-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5576-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5576-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5576-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f5576-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5576-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f5576-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5576-115">Not supported.</span></span>|
|<span data-ttu-id="f5576-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5576-116">Application</span></span>|<span data-ttu-id="f5576-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5576-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f5576-118">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f5576-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f5576-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f5576-119">Global administrator</span></span>
* <span data-ttu-id="f5576-120">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="f5576-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f5576-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5576-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5576-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5576-122">Request headers</span></span>

|<span data-ttu-id="f5576-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f5576-123">Name</span></span>|<span data-ttu-id="f5576-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f5576-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5576-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5576-125">Authorization</span></span>|<span data-ttu-id="f5576-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5576-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5576-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5576-128">Request body</span></span>

<span data-ttu-id="f5576-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5576-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5576-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5576-130">Response</span></span>

<span data-ttu-id="f5576-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5576-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f5576-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="f5576-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5576-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5576-133">Request</span></span>

<span data-ttu-id="f5576-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5576-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f5576-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5576-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```
# <a name="c"></a>[<span data-ttu-id="f5576-136">C#</span><span class="sxs-lookup"><span data-stu-id="f5576-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5576-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5576-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5576-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5576-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5576-139">Java</span><span class="sxs-lookup"><span data-stu-id="f5576-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5576-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5576-140">Response</span></span>

<span data-ttu-id="f5576-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5576-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
