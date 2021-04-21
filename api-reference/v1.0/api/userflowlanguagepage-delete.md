---
title: Удаление userFlowLanguagePage
description: Удаляет значения в объекте userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6ae4c73b2b76b519190a1cd5fdb4d25644684952
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920506"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="01181-103">Удаление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="01181-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="01181-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01181-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01181-105">Удаляет значения в [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="01181-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="01181-106">Можно удалить только значения в переопределеченной странице, которая используется для настройки значений, показанных пользователю во время пользовательского пути, определенного потоком пользователей.</span><span class="sxs-lookup"><span data-stu-id="01181-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="01181-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01181-107">Permissions</span></span>

<span data-ttu-id="01181-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01181-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01181-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01181-110">Permission type</span></span>      | <span data-ttu-id="01181-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01181-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01181-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01181-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01181-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01181-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="01181-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01181-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="01181-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01181-115">Not supported.</span></span>|
|<span data-ttu-id="01181-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01181-116">Application</span></span>|<span data-ttu-id="01181-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01181-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="01181-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="01181-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="01181-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="01181-119">Global administrator</span></span>
* <span data-ttu-id="01181-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="01181-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="01181-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01181-121">HTTP request</span></span>

<span data-ttu-id="01181-122">Чтобы ссылаться на содержимое объекта, необходимо использовать `$value` .</span><span class="sxs-lookup"><span data-stu-id="01181-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="01181-123">Это возвращает содержимое объекта и позволяет ссылаться на него напрямую.</span><span class="sxs-lookup"><span data-stu-id="01181-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="01181-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01181-124">Request headers</span></span>

|<span data-ttu-id="01181-125">Имя</span><span class="sxs-lookup"><span data-stu-id="01181-125">Name</span></span>|<span data-ttu-id="01181-126">Описание</span><span class="sxs-lookup"><span data-stu-id="01181-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="01181-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01181-127">Authorization</span></span>|<span data-ttu-id="01181-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01181-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01181-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01181-130">Request body</span></span>

<span data-ttu-id="01181-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01181-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01181-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="01181-132">Response</span></span>

<span data-ttu-id="01181-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01181-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="01181-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="01181-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01181-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="01181-135">Request</span></span>

<span data-ttu-id="01181-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01181-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="01181-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="01181-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
```
# <a name="c"></a>[<span data-ttu-id="01181-138">C#</span><span class="sxs-lookup"><span data-stu-id="01181-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01181-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01181-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01181-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01181-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01181-141">Java</span><span class="sxs-lookup"><span data-stu-id="01181-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01181-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="01181-142">Response</span></span>

<span data-ttu-id="01181-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01181-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
