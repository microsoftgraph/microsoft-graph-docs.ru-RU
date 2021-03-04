---
title: Обновление continuousAccessEvaluationPolicy
description: Обновление свойств объекта continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 80c08c4b711daa2e79600c20ce11f30cd7879af4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437284"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="1dbc9-103">Обновление continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="1dbc9-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="1dbc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dbc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dbc9-105">Обновление свойств объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1dbc9-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dbc9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbc9-106">Permissions</span></span>
<span data-ttu-id="1dbc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dbc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbc9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbc9-109">Permission type</span></span>                        | <span data-ttu-id="1dbc9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dbc9-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="1dbc9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dbc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dbc9-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dbc9-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="1dbc9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dbc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dbc9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-114">Not supported.</span></span> |
|<span data-ttu-id="1dbc9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1dbc9-115">Application</span></span>                            | <span data-ttu-id="1dbc9-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dbc9-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="1dbc9-117">Этот API имеет [известные проблемы, связанные](/graph/known-issues#permissions) с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dbc9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dbc9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="1dbc9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dbc9-119">Request headers</span></span>
|<span data-ttu-id="1dbc9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1dbc9-120">Name</span></span>|<span data-ttu-id="1dbc9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1dbc9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1dbc9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dbc9-122">Authorization</span></span>|<span data-ttu-id="1dbc9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1dbc9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dbc9-125">Content-Type</span></span>|<span data-ttu-id="1dbc9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbc9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dbc9-128">Request body</span></span>
<span data-ttu-id="1dbc9-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1dbc9-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1dbc9-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="1dbc9-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dbc9-132">Property</span></span>|<span data-ttu-id="1dbc9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1dbc9-133">Type</span></span>|<span data-ttu-id="1dbc9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1dbc9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbc9-135">groups</span><span class="sxs-lookup"><span data-stu-id="1dbc9-135">groups</span></span>|<span data-ttu-id="1dbc9-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1dbc9-136">String collection</span></span>|<span data-ttu-id="1dbc9-137">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="1dbc9-138">Все группы находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="1dbc9-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1dbc9-139">isEnabled</span></span>|<span data-ttu-id="1dbc9-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dbc9-140">Boolean</span></span>| <span data-ttu-id="1dbc9-141">`true` указать, следует ли проводить оценку непрерывного доступа; в противном `false` случае .</span><span class="sxs-lookup"><span data-stu-id="1dbc9-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="1dbc9-142">users</span><span class="sxs-lookup"><span data-stu-id="1dbc9-142">users</span></span>|<span data-ttu-id="1dbc9-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1dbc9-143">String collection</span></span>|<span data-ttu-id="1dbc9-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="1dbc9-145">Все пользователи находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="1dbc9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbc9-146">Response</span></span>

<span data-ttu-id="1dbc9-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dbc9-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="1dbc9-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1dbc9-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dbc9-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dbc9-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dbc9-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```
# <a name="c"></a>[<span data-ttu-id="1dbc9-152">C#</span><span class="sxs-lookup"><span data-stu-id="1dbc9-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dbc9-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dbc9-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dbc9-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dbc9-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dbc9-155">Java</span><span class="sxs-lookup"><span data-stu-id="1dbc9-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1dbc9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbc9-156">Response</span></span>

<span data-ttu-id="1dbc9-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1dbc9-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
