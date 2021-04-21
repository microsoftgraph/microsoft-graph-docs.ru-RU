---
title: Get userFlowLanguagePage
description: Чтение значений в объекте userFlowLanguagePage для языка в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bf35e829e0c5f8cc9df6af502962aab4a6a4a83b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920479"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="247b5-103">Get userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="247b5-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="247b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="247b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="247b5-105">Чтение значений в [объекте userFlowLanguagePage](../resources/userflowlanguagepage.md) для языка в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="247b5-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="247b5-106">Эти значения показаны пользователю во время путешествия пользователя, определенного потоком пользователей.</span><span class="sxs-lookup"><span data-stu-id="247b5-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="247b5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="247b5-107">Permissions</span></span>

<span data-ttu-id="247b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="247b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="247b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="247b5-110">Permission type</span></span>      | <span data-ttu-id="247b5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="247b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="247b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="247b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="247b5-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247b5-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="247b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="247b5-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="247b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="247b5-115">Not supported.</span></span>|
|<span data-ttu-id="247b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="247b5-116">Application</span></span>|<span data-ttu-id="247b5-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247b5-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="247b5-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="247b5-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="247b5-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="247b5-119">Global administrator</span></span>
* <span data-ttu-id="247b5-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="247b5-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="247b5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="247b5-121">HTTP request</span></span>

<span data-ttu-id="247b5-122">Чтобы ссылаться на содержимое объекта, необходимо использовать `$value` .</span><span class="sxs-lookup"><span data-stu-id="247b5-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="247b5-123">Это возвращает содержимое объекта и позволяет ссылаться на него напрямую.</span><span class="sxs-lookup"><span data-stu-id="247b5-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="247b5-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="247b5-124">Request headers</span></span>

|<span data-ttu-id="247b5-125">Имя</span><span class="sxs-lookup"><span data-stu-id="247b5-125">Name</span></span>|<span data-ttu-id="247b5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="247b5-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="247b5-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="247b5-127">Authorization</span></span>|<span data-ttu-id="247b5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="247b5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="247b5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="247b5-130">Request body</span></span>

<span data-ttu-id="247b5-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="247b5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="247b5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="247b5-132">Response</span></span>

<span data-ttu-id="247b5-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="247b5-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="247b5-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="247b5-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="247b5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="247b5-135">Request</span></span>

<span data-ttu-id="247b5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="247b5-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="247b5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="247b5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value
```
# <a name="c"></a>[<span data-ttu-id="247b5-138">C#</span><span class="sxs-lookup"><span data-stu-id="247b5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="247b5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="247b5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="247b5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="247b5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="247b5-141">Java</span><span class="sxs-lookup"><span data-stu-id="247b5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="247b5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="247b5-142">Response</span></span>

<span data-ttu-id="247b5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="247b5-143">The following is an example of the response.</span></span>

<span data-ttu-id="247b5-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="247b5-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ErrorMessage",
        "ElementId": null,
        "StringId": "ServiceThrottled",
        "Override": false,
        "Value": "There are too many requests at this moment. Please wait for some time and try again."
      }
   ]
}
```
