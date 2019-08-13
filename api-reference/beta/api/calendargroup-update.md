---
title: Обновление объекта calendarGroup.
description: Обновление свойств объекта calendarGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 830e985d806108a3eeac9581d5c54e7f9bba8dd4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317824"
---
# <a name="update-calendargroup"></a><span data-ttu-id="bde9d-103">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="bde9d-103">Update calendargroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bde9d-104">Обновление свойств объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="bde9d-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bde9d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bde9d-105">Permissions</span></span>

<span data-ttu-id="bde9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bde9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bde9d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bde9d-108">Permission type</span></span>                        | <span data-ttu-id="bde9d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bde9d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bde9d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bde9d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bde9d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bde9d-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bde9d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bde9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bde9d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bde9d-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bde9d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bde9d-114">Application</span></span>                            | <span data-ttu-id="bde9d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bde9d-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bde9d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bde9d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="bde9d-117">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="bde9d-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bde9d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bde9d-118">Request headers</span></span>

| <span data-ttu-id="bde9d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bde9d-119">Header</span></span>        | <span data-ttu-id="bde9d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bde9d-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="bde9d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bde9d-121">Authorization</span></span> | <span data-ttu-id="bde9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bde9d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bde9d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bde9d-124">Content-Type</span></span>  | <span data-ttu-id="bde9d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bde9d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bde9d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bde9d-127">Request body</span></span>

<span data-ttu-id="bde9d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bde9d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bde9d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="bde9d-131">Property</span></span> | <span data-ttu-id="bde9d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="bde9d-132">Type</span></span>   | <span data-ttu-id="bde9d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bde9d-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="bde9d-134">name</span><span class="sxs-lookup"><span data-stu-id="bde9d-134">name</span></span>     | <span data-ttu-id="bde9d-135">String</span><span class="sxs-lookup"><span data-stu-id="bde9d-135">String</span></span> | <span data-ttu-id="bde9d-136">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="bde9d-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="bde9d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bde9d-137">Response</span></span>

<span data-ttu-id="bde9d-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bde9d-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bde9d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="bde9d-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bde9d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bde9d-140">Request</span></span>

<span data-ttu-id="bde9d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bde9d-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bde9d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bde9d-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bde9d-143">C#</span><span class="sxs-lookup"><span data-stu-id="bde9d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bde9d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bde9d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bde9d-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bde9d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bde9d-146">Java</span><span class="sxs-lookup"><span data-stu-id="bde9d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bde9d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bde9d-147">Response</span></span>

<span data-ttu-id="bde9d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bde9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
