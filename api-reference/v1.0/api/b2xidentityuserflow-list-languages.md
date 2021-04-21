---
title: Перечисление языков
description: Извлечение списка языков, поддерживаемых для настройки в потоке пользователей B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 21f2611fe61d1a4165ba1fe0896f711869809aea
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919903"
---
# <a name="list-languages"></a><span data-ttu-id="6dced-103">Перечисление языков</span><span class="sxs-lookup"><span data-stu-id="6dced-103">List languages</span></span>

<span data-ttu-id="6dced-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dced-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dced-105">Извлечение списка языков, поддерживаемых для настройки в потоке пользователей B2X.</span><span class="sxs-lookup"><span data-stu-id="6dced-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dced-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dced-106">Permissions</span></span>

<span data-ttu-id="6dced-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dced-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dced-109">Permission type</span></span>      | <span data-ttu-id="6dced-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dced-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dced-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dced-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dced-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dced-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6dced-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dced-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6dced-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dced-114">Not supported.</span></span>|
|<span data-ttu-id="6dced-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6dced-115">Application</span></span>|<span data-ttu-id="6dced-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dced-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6dced-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6dced-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6dced-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6dced-118">Global administrator</span></span>
* <span data-ttu-id="6dced-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="6dced-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6dced-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dced-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="6dced-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dced-121">Request headers</span></span>

|<span data-ttu-id="6dced-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6dced-122">Name</span></span>|<span data-ttu-id="6dced-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6dced-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dced-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dced-124">Authorization</span></span>|<span data-ttu-id="6dced-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dced-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dced-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dced-127">Request body</span></span>

<span data-ttu-id="6dced-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dced-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dced-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dced-129">Response</span></span>

<span data-ttu-id="6dced-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6dced-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dced-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dced-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dced-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dced-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6dced-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dced-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="6dced-134">C#</span><span class="sxs-lookup"><span data-stu-id="6dced-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dced-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dced-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dced-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dced-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6dced-137">Java</span><span class="sxs-lookup"><span data-stu-id="6dced-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6dced-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dced-138">Response</span></span>

<span data-ttu-id="6dced-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dced-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
