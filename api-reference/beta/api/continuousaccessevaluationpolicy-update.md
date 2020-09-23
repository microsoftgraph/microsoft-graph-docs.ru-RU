---
title: Обновление Континуаусакцессевалуатионполици
description: Обновление свойств объекта Континуаусакцессевалуатионполици.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2838a02481690db3d81fd544e88fce65b2053495
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223143"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="64f77-103">Обновление Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="64f77-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="64f77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f77-105">Обновление свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="64f77-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64f77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64f77-106">Permissions</span></span>
<span data-ttu-id="64f77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f77-109">Permission type</span></span>                        | <span data-ttu-id="64f77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f77-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="64f77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f77-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64f77-112">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="64f77-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="64f77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f77-114">Not supported.</span></span> |
|<span data-ttu-id="64f77-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="64f77-115">Application</span></span>                            | <span data-ttu-id="64f77-116">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="64f77-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="64f77-117">У этого API есть [известная проблема](/graph/known-issues#permissions) , связанная с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="64f77-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="64f77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f77-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="64f77-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64f77-119">Request headers</span></span>
|<span data-ttu-id="64f77-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64f77-120">Name</span></span>|<span data-ttu-id="64f77-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64f77-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64f77-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f77-122">Authorization</span></span>|<span data-ttu-id="64f77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f77-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64f77-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64f77-125">Content-Type</span></span>|<span data-ttu-id="64f77-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f77-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f77-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64f77-128">Request body</span></span>
<span data-ttu-id="64f77-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="64f77-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="64f77-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="64f77-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="64f77-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="64f77-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="64f77-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f77-132">Property</span></span>|<span data-ttu-id="64f77-133">Тип</span><span class="sxs-lookup"><span data-stu-id="64f77-133">Type</span></span>|<span data-ttu-id="64f77-134">Описание</span><span class="sxs-lookup"><span data-stu-id="64f77-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f77-135">groups</span><span class="sxs-lookup"><span data-stu-id="64f77-135">groups</span></span>|<span data-ttu-id="64f77-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64f77-136">String collection</span></span>|<span data-ttu-id="64f77-137">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="64f77-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="64f77-138">Если коллекция пуста, все группы находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="64f77-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="64f77-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="64f77-139">isEnabled</span></span>|<span data-ttu-id="64f77-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f77-140">Boolean</span></span>| <span data-ttu-id="64f77-141">`true` , чтобы указать, следует ли выполнять оценку непрерывного доступа; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="64f77-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="64f77-142">users</span><span class="sxs-lookup"><span data-stu-id="64f77-142">users</span></span>|<span data-ttu-id="64f77-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64f77-143">String collection</span></span>|<span data-ttu-id="64f77-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="64f77-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="64f77-145">Если коллекция пуста, все пользователи находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="64f77-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="64f77-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f77-146">Response</span></span>

<span data-ttu-id="64f77-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64f77-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64f77-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="64f77-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64f77-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f77-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64f77-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="64f77-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="64f77-152">C#</span><span class="sxs-lookup"><span data-stu-id="64f77-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64f77-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64f77-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64f77-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64f77-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64f77-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f77-155">Response</span></span>

<span data-ttu-id="64f77-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64f77-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
