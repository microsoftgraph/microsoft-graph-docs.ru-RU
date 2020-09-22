---
title: Обновление Континуаусакцессевалуатионполици
description: Обновление свойств объекта Континуаусакцессевалуатионполици.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6a3cbffdb8058051442b85aeb6617639ce5dd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023540"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="8d9e0-103">Обновление Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="8d9e0-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="8d9e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d9e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d9e0-105">Обновление свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8d9e0-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d9e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d9e0-106">Permissions</span></span>
<span data-ttu-id="8d9e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d9e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d9e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d9e0-109">Permission type</span></span>                        | <span data-ttu-id="8d9e0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d9e0-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="8d9e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d9e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d9e0-112">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8d9e0-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="8d9e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d9e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d9e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-114">Not supported.</span></span> |
|<span data-ttu-id="8d9e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d9e0-115">Application</span></span>                            | <span data-ttu-id="8d9e0-116">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8d9e0-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="8d9e0-117">У этого API есть [известная проблема](/graph/known-issues#permissions) , связанная с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d9e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d9e0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="8d9e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d9e0-119">Request headers</span></span>
|<span data-ttu-id="8d9e0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8d9e0-120">Name</span></span>|<span data-ttu-id="8d9e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8d9e0-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d9e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d9e0-122">Authorization</span></span>|<span data-ttu-id="8d9e0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8d9e0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d9e0-125">Content-Type</span></span>|<span data-ttu-id="8d9e0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d9e0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d9e0-128">Request body</span></span>
<span data-ttu-id="8d9e0-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8d9e0-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8d9e0-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="8d9e0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d9e0-132">Property</span></span>|<span data-ttu-id="8d9e0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8d9e0-133">Type</span></span>|<span data-ttu-id="8d9e0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8d9e0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d9e0-135">groups</span><span class="sxs-lookup"><span data-stu-id="8d9e0-135">groups</span></span>|<span data-ttu-id="8d9e0-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8d9e0-136">String collection</span></span>|<span data-ttu-id="8d9e0-137">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="8d9e0-138">Если коллекция пуста, все группы находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="8d9e0-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8d9e0-139">isEnabled</span></span>|<span data-ttu-id="8d9e0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d9e0-140">Boolean</span></span>| <span data-ttu-id="8d9e0-141">`true` , чтобы указать, следует ли выполнять оценку непрерывного доступа; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="8d9e0-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="8d9e0-142">users</span><span class="sxs-lookup"><span data-stu-id="8d9e0-142">users</span></span>|<span data-ttu-id="8d9e0-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8d9e0-143">String collection</span></span>|<span data-ttu-id="8d9e0-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="8d9e0-145">Если коллекция пуста, все пользователи находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="8d9e0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d9e0-146">Response</span></span>

<span data-ttu-id="8d9e0-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d9e0-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d9e0-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d9e0-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d9e0-150">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="8d9e0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d9e0-151">Response</span></span>

<span data-ttu-id="8d9e0-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d9e0-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```