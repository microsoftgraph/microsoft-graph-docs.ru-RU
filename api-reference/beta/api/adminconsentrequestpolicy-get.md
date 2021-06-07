---
title: Получить adminConsentRequestPolicy
description: Ознакомьтесь с свойствами и отношениями объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 78a9696a036b0cbd246dfaa03e5ba7f3c6e6a8cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751003"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="8f50d-103">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="8f50d-103">Get adminConsentRequestPolicy</span></span>
<span data-ttu-id="8f50d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f50d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f50d-105">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f50d-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f50d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f50d-106">Permissions</span></span>
<span data-ttu-id="8f50d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f50d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f50d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f50d-109">Permission type</span></span>|<span data-ttu-id="8f50d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f50d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f50d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f50d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f50d-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f50d-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="8f50d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f50d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f50d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f50d-114">Not supported.</span></span>|
|<span data-ttu-id="8f50d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f50d-115">Application</span></span>|<span data-ttu-id="8f50d-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f50d-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="8f50d-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="8f50d-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="8f50d-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="8f50d-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="8f50d-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8f50d-119">Global Administrator</span></span>
+ <span data-ttu-id="8f50d-120">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="8f50d-120">Global Reader</span></span>
+ <span data-ttu-id="8f50d-121">Администратор облачного приложения</span><span class="sxs-lookup"><span data-stu-id="8f50d-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="8f50d-122">Администратор приложения</span><span class="sxs-lookup"><span data-stu-id="8f50d-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8f50d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f50d-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f50d-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f50d-124">Optional query parameters</span></span>
<span data-ttu-id="8f50d-125">Этот метод поддерживает параметр  `$select`   запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f50d-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="8f50d-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8f50d-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f50d-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f50d-127">Request headers</span></span>
|<span data-ttu-id="8f50d-128">Имя</span><span class="sxs-lookup"><span data-stu-id="8f50d-128">Name</span></span>|<span data-ttu-id="8f50d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8f50d-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f50d-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f50d-130">Authorization</span></span>|<span data-ttu-id="8f50d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f50d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f50d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f50d-133">Request body</span></span>
<span data-ttu-id="8f50d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f50d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f50d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f50d-135">Response</span></span>

<span data-ttu-id="8f50d-136">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8f50d-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f50d-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f50d-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f50d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f50d-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8f50d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f50d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy
```
# <a name="c"></a>[<span data-ttu-id="8f50d-140">C#</span><span class="sxs-lookup"><span data-stu-id="8f50d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f50d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f50d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f50d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f50d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f50d-143">Java</span><span class="sxs-lookup"><span data-stu-id="8f50d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8f50d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f50d-144">Response</span></span>
><span data-ttu-id="8f50d-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8f50d-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": false,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": []
}
```
