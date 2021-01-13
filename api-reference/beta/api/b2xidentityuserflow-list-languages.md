---
title: Перечисление языков
description: Получить список языков, поддерживаемых для настройки в пользовательском потоке B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 523b9c09b879e6d9938e08d96714dd9a709a3a85
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843642"
---
# <a name="list-languages"></a><span data-ttu-id="70b3b-103">Перечисление языков</span><span class="sxs-lookup"><span data-stu-id="70b3b-103">List languages</span></span>

<span data-ttu-id="70b3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70b3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70b3b-105">Получить список языков, поддерживаемых для настройки в пользовательском потоке B2X.</span><span class="sxs-lookup"><span data-stu-id="70b3b-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="70b3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70b3b-106">Permissions</span></span>

<span data-ttu-id="70b3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70b3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70b3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70b3b-109">Permission type</span></span>      | <span data-ttu-id="70b3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70b3b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70b3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70b3b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70b3b-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b3b-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="70b3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70b3b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="70b3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70b3b-114">Not supported.</span></span>|
|<span data-ttu-id="70b3b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="70b3b-115">Application</span></span>|<span data-ttu-id="70b3b-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b3b-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="70b3b-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="70b3b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="70b3b-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="70b3b-118">Global administrator</span></span>
* <span data-ttu-id="70b3b-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="70b3b-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="70b3b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70b3b-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="70b3b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70b3b-121">Request headers</span></span>

|<span data-ttu-id="70b3b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="70b3b-122">Name</span></span>|<span data-ttu-id="70b3b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="70b3b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70b3b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70b3b-124">Authorization</span></span>|<span data-ttu-id="70b3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70b3b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70b3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70b3b-127">Request body</span></span>

<span data-ttu-id="70b3b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70b3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70b3b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="70b3b-129">Response</span></span>

<span data-ttu-id="70b3b-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70b3b-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70b3b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="70b3b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70b3b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70b3b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70b3b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70b3b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="70b3b-134">C#</span><span class="sxs-lookup"><span data-stu-id="70b3b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70b3b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70b3b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70b3b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70b3b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70b3b-137">Java</span><span class="sxs-lookup"><span data-stu-id="70b3b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70b3b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="70b3b-138">Response</span></span>

<span data-ttu-id="70b3b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70b3b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
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
