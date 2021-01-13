---
title: Список defaultPages
description: Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5339bebc87223fb6ca055fa0c1801bdffbd3edc1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844944"
---
# <a name="list-defaultpages"></a><span data-ttu-id="93d9b-103">Список defaultPages</span><span class="sxs-lookup"><span data-stu-id="93d9b-103">List defaultPages</span></span>

<span data-ttu-id="93d9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93d9b-105">Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.</span><span class="sxs-lookup"><span data-stu-id="93d9b-105">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="93d9b-106">Они содержат значения, показанные пользователю в пользовательском пути по умолчанию для пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="93d9b-106">These contain the values shown to the user in a default user journey of a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d9b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93d9b-107">Permissions</span></span>

<span data-ttu-id="93d9b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d9b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93d9b-110">Permission type</span></span>      | <span data-ttu-id="93d9b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93d9b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d9b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93d9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93d9b-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d9b-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="93d9b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93d9b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="93d9b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d9b-115">Not supported.</span></span>|
|<span data-ttu-id="93d9b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="93d9b-116">Application</span></span>|<span data-ttu-id="93d9b-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d9b-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="93d9b-118">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="93d9b-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="93d9b-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="93d9b-119">Global administrator</span></span>
* <span data-ttu-id="93d9b-120">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="93d9b-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="93d9b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93d9b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages
```

## <a name="request-headers"></a><span data-ttu-id="93d9b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93d9b-122">Request headers</span></span>

|<span data-ttu-id="93d9b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="93d9b-123">Name</span></span>|<span data-ttu-id="93d9b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="93d9b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="93d9b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93d9b-125">Authorization</span></span>|<span data-ttu-id="93d9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93d9b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93d9b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93d9b-128">Request body</span></span>

<span data-ttu-id="93d9b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93d9b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d9b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d9b-130">Response</span></span>

<span data-ttu-id="93d9b-131">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93d9b-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93d9b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="93d9b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93d9b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d9b-133">Request</span></span>

<span data-ttu-id="93d9b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d9b-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93d9b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="93d9b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages
```
# <a name="c"></a>[<span data-ttu-id="93d9b-136">C#</span><span class="sxs-lookup"><span data-stu-id="93d9b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93d9b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93d9b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93d9b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93d9b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93d9b-139">Java</span><span class="sxs-lookup"><span data-stu-id="93d9b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93d9b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d9b-140">Response</span></span>

<span data-ttu-id="93d9b-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93d9b-141">The following is an example of the response.</span></span>

<span data-ttu-id="93d9b-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93d9b-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
