---
title: Переопределения списка
description: Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 130710b0c1be9ad2b46a73aeeb80f319c5d4adde
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444660"
---
# <a name="list-overridespages"></a><span data-ttu-id="65b26-103">Переопределения списка</span><span class="sxs-lookup"><span data-stu-id="65b26-103">List overridesPages</span></span>

<span data-ttu-id="65b26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65b26-105">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="65b26-105">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="65b26-106">Эти страницы используются для настройки значений, показанных пользователю во время пользовательского пути в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="65b26-106">These pages are used to customize the values shown to the user during a user journey in a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b26-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65b26-107">Permissions</span></span>

<span data-ttu-id="65b26-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b26-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65b26-110">Permission type</span></span>      | <span data-ttu-id="65b26-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65b26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b26-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65b26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65b26-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b26-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="65b26-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65b26-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="65b26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65b26-115">Not supported.</span></span>|
|<span data-ttu-id="65b26-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="65b26-116">Application</span></span>|<span data-ttu-id="65b26-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b26-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="65b26-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="65b26-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="65b26-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="65b26-119">Global administrator</span></span>
* <span data-ttu-id="65b26-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="65b26-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="65b26-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65b26-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages
```

## <a name="request-headers"></a><span data-ttu-id="65b26-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65b26-122">Request headers</span></span>

|<span data-ttu-id="65b26-123">Имя</span><span class="sxs-lookup"><span data-stu-id="65b26-123">Name</span></span>|<span data-ttu-id="65b26-124">Описание</span><span class="sxs-lookup"><span data-stu-id="65b26-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65b26-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65b26-125">Authorization</span></span>|<span data-ttu-id="65b26-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65b26-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b26-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65b26-128">Request body</span></span>

<span data-ttu-id="65b26-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65b26-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b26-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b26-130">Response</span></span>

<span data-ttu-id="65b26-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65b26-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65b26-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="65b26-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65b26-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="65b26-133">Request</span></span>

<span data-ttu-id="65b26-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65b26-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="65b26-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b26-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages
```
# <a name="c"></a>[<span data-ttu-id="65b26-136">C#</span><span class="sxs-lookup"><span data-stu-id="65b26-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65b26-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b26-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b26-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b26-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65b26-139">Java</span><span class="sxs-lookup"><span data-stu-id="65b26-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65b26-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b26-140">Response</span></span>

<span data-ttu-id="65b26-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65b26-141">The following is an example of the response.</span></span>

<span data-ttu-id="65b26-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65b26-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "idpselections"
    },
    {
      "id": "phonefactor"
    }
  ]
}
```
