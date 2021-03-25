---
title: Обновление adminConsentRequestPolicy
description: Обновление свойств объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3fcd6bb895a4f1cb36f099269c8414669dc98620
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201495"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="97119-103">Обновление adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="97119-103">Update adminConsentRequestPolicy</span></span>
<span data-ttu-id="97119-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97119-105">Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97119-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97119-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97119-106">Permissions</span></span>
<span data-ttu-id="97119-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97119-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97119-109">Permission type</span></span>|<span data-ttu-id="97119-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97119-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97119-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97119-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97119-112">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="97119-112">Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="97119-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97119-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97119-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97119-114">Not supported.</span></span>|
|<span data-ttu-id="97119-115">Application</span><span class="sxs-lookup"><span data-stu-id="97119-115">Application</span></span>|<span data-ttu-id="97119-116">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="97119-116">Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="97119-117">При вызове от имени пользователя пользователю необходимо принадлежать к роли [глобального](/azure/active-directory/roles/permissions-reference) администратора.</span><span class="sxs-lookup"><span data-stu-id="97119-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="97119-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97119-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy 
```

## <a name="request-headers"></a><span data-ttu-id="97119-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97119-119">Request headers</span></span>
|<span data-ttu-id="97119-120">Имя</span><span class="sxs-lookup"><span data-stu-id="97119-120">Name</span></span>|<span data-ttu-id="97119-121">Описание</span><span class="sxs-lookup"><span data-stu-id="97119-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97119-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97119-122">Authorization</span></span>|<span data-ttu-id="97119-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97119-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97119-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97119-125">Content-Type</span></span>|<span data-ttu-id="97119-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97119-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97119-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97119-128">Request body</span></span>
<span data-ttu-id="97119-129">В теле запроса поставляют представление JSON объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97119-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="97119-130">В следующей таблице показаны свойства, необходимые при обновлении [администрированияConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97119-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="97119-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="97119-131">Property</span></span>|<span data-ttu-id="97119-132">Тип</span><span class="sxs-lookup"><span data-stu-id="97119-132">Type</span></span>|<span data-ttu-id="97119-133">Описание</span><span class="sxs-lookup"><span data-stu-id="97119-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97119-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="97119-134">isEnabled</span></span>|<span data-ttu-id="97119-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="97119-135">Boolean</span></span>|<span data-ttu-id="97119-136">Указывает, включена или отключена функция запроса на согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="97119-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="97119-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="97119-137">notifyReviewers</span></span>|<span data-ttu-id="97119-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="97119-138">Boolean</span></span>|<span data-ttu-id="97119-139">Указывает, будут ли рецензенты получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="97119-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="97119-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="97119-140">remindersEnabled</span></span>|<span data-ttu-id="97119-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="97119-141">Boolean</span></span>|<span data-ttu-id="97119-142">Указывает, будут ли рецензенты получать сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="97119-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="97119-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="97119-143">requestDurationInDays</span></span>|<span data-ttu-id="97119-144">Int32</span><span class="sxs-lookup"><span data-stu-id="97119-144">Int32</span></span>|<span data-ttu-id="97119-145">Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.</span><span class="sxs-lookup"><span data-stu-id="97119-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="97119-146">рецензенты</span><span class="sxs-lookup"><span data-stu-id="97119-146">reviewers</span></span>|<span data-ttu-id="97119-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="97119-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="97119-148">Список рецензентов для согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="97119-148">The list of reviewers for the admin consent.</span></span>|



## <a name="response"></a><span data-ttu-id="97119-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="97119-149">Response</span></span>

<span data-ttu-id="97119-150">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="97119-150">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="97119-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="97119-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97119-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="97119-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97119-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="97119-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="97119-154">C#</span><span class="sxs-lookup"><span data-stu-id="97119-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97119-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97119-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97119-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97119-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97119-157">Java</span><span class="sxs-lookup"><span data-stu-id="97119-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="97119-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="97119-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
