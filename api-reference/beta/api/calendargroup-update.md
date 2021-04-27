---
title: Обновление объекта calendarGroup.
description: Обновление свойств объекта calendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9395d46f587aa49ed4f77dbe47d2b971e2baeb56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047695"
---
# <a name="update-calendargroup"></a><span data-ttu-id="418ac-103">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="418ac-103">Update calendargroup</span></span>

<span data-ttu-id="418ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="418ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418ac-105">Обновление свойств объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="418ac-105">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="418ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="418ac-106">Permissions</span></span>

<span data-ttu-id="418ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="418ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="418ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="418ac-109">Permission type</span></span>                        | <span data-ttu-id="418ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="418ac-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="418ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="418ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="418ac-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="418ac-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="418ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="418ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="418ac-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="418ac-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="418ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="418ac-115">Application</span></span>                            | <span data-ttu-id="418ac-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="418ac-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="418ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="418ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="418ac-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="418ac-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="418ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="418ac-119">Request headers</span></span>

| <span data-ttu-id="418ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="418ac-120">Header</span></span>        | <span data-ttu-id="418ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="418ac-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="418ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="418ac-122">Authorization</span></span> | <span data-ttu-id="418ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418ac-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="418ac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="418ac-125">Content-Type</span></span>  | <span data-ttu-id="418ac-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418ac-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="418ac-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="418ac-128">Request body</span></span>

<span data-ttu-id="418ac-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="418ac-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="418ac-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="418ac-132">Property</span></span> | <span data-ttu-id="418ac-133">Тип</span><span class="sxs-lookup"><span data-stu-id="418ac-133">Type</span></span>   | <span data-ttu-id="418ac-134">Описание</span><span class="sxs-lookup"><span data-stu-id="418ac-134">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="418ac-135">name</span><span class="sxs-lookup"><span data-stu-id="418ac-135">name</span></span>     | <span data-ttu-id="418ac-136">String</span><span class="sxs-lookup"><span data-stu-id="418ac-136">String</span></span> | <span data-ttu-id="418ac-137">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="418ac-137">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="418ac-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="418ac-138">Response</span></span>

<span data-ttu-id="418ac-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="418ac-139">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418ac-140">Пример</span><span class="sxs-lookup"><span data-stu-id="418ac-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="418ac-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="418ac-141">Request</span></span>

<span data-ttu-id="418ac-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="418ac-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="418ac-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="418ac-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="418ac-144">C#</span><span class="sxs-lookup"><span data-stu-id="418ac-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="418ac-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="418ac-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="418ac-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="418ac-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="418ac-147">Java</span><span class="sxs-lookup"><span data-stu-id="418ac-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="418ac-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="418ac-148">Response</span></span>

<span data-ttu-id="418ac-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="418ac-149">Here is an example of the response.</span></span> <span data-ttu-id="418ac-150">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="418ac-150">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


