---
title: Получить adminConsentRequestPolicy
description: Ознакомьтесь с свойствами и отношениями объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3c50b0a3197e682d00688ab8ec3527ed279aefa8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201500"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="21357-103">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="21357-103">Get adminConsentRequestPolicy</span></span>
<span data-ttu-id="21357-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21357-105">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21357-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21357-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21357-106">Permissions</span></span>
<span data-ttu-id="21357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21357-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21357-109">Permission type</span></span>|<span data-ttu-id="21357-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21357-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21357-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21357-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21357-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="21357-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="21357-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21357-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21357-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21357-114">Not supported.</span></span>|
|<span data-ttu-id="21357-115">Application</span><span class="sxs-lookup"><span data-stu-id="21357-115">Application</span></span>|<span data-ttu-id="21357-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="21357-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="21357-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="21357-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="21357-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="21357-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="21357-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="21357-119">Global Administrator</span></span>
+ <span data-ttu-id="21357-120">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="21357-120">Global Reader</span></span>
+ <span data-ttu-id="21357-121">Администратор облачного приложения</span><span class="sxs-lookup"><span data-stu-id="21357-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="21357-122">Администратор приложения</span><span class="sxs-lookup"><span data-stu-id="21357-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="21357-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21357-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21357-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21357-124">Optional query parameters</span></span>
<span data-ttu-id="21357-125">Этот метод поддерживает параметр  `$select`   запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="21357-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="21357-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="21357-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="21357-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21357-127">Request headers</span></span>
|<span data-ttu-id="21357-128">Имя</span><span class="sxs-lookup"><span data-stu-id="21357-128">Name</span></span>|<span data-ttu-id="21357-129">Описание</span><span class="sxs-lookup"><span data-stu-id="21357-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="21357-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21357-130">Authorization</span></span>|<span data-ttu-id="21357-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21357-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21357-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21357-133">Request body</span></span>
<span data-ttu-id="21357-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21357-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21357-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="21357-135">Response</span></span>

<span data-ttu-id="21357-136">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21357-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21357-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="21357-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21357-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="21357-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="21357-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="21357-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy
```
# <a name="c"></a>[<span data-ttu-id="21357-140">C#</span><span class="sxs-lookup"><span data-stu-id="21357-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21357-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21357-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21357-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21357-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21357-143">Java</span><span class="sxs-lookup"><span data-stu-id="21357-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="21357-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="21357-144">Response</span></span>
<span data-ttu-id="21357-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21357-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
