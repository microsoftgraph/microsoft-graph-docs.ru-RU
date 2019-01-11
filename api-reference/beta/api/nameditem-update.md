---
title: Обновление объекта NamedItem
description: Обновление свойств объекта nameditem.
localization_priority: Normal
ms.openlocfilehash: b7ef5b2086668b525cf527baab5a882f9c11e6ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883750"
---
# <a name="update-nameditem"></a><span data-ttu-id="c9f5b-103">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="c9f5b-103">Update nameditem</span></span>

> <span data-ttu-id="c9f5b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9f5b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9f5b-106">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-106">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9f5b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9f5b-107">Permissions</span></span>
<span data-ttu-id="c9f5b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9f5b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9f5b-110">Permission type</span></span>      | <span data-ttu-id="c9f5b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9f5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9f5b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9f5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9f5b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9f5b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9f5b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9f5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9f5b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9f5b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9f5b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9f5b-116">Application</span></span> | <span data-ttu-id="c9f5b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9f5b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9f5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="c9f5b-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9f5b-119">Optional request headers</span></span>
| <span data-ttu-id="c9f5b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c9f5b-120">Name</span></span>       | <span data-ttu-id="c9f5b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c9f5b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c9f5b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9f5b-122">Authorization</span></span>  | <span data-ttu-id="c9f5b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9f5b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c9f5b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c9f5b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9f5b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9f5b-128">Request body</span></span>
<span data-ttu-id="c9f5b-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9f5b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9f5b-132">Property</span></span>     | <span data-ttu-id="c9f5b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c9f5b-133">Type</span></span>   |<span data-ttu-id="c9f5b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c9f5b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9f5b-135">visible</span><span class="sxs-lookup"><span data-stu-id="c9f5b-135">visible</span></span>|<span data-ttu-id="c9f5b-136">boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-136">boolean</span></span>|<span data-ttu-id="c9f5b-137">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-137">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="c9f5b-138">comment</span><span class="sxs-lookup"><span data-stu-id="c9f5b-138">comment</span></span>|   <span data-ttu-id="c9f5b-139">строка</span><span class="sxs-lookup"><span data-stu-id="c9f5b-139">string</span></span>  |<span data-ttu-id="c9f5b-140">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-140">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="c9f5b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9f5b-141">Response</span></span>

<span data-ttu-id="c9f5b-142">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-142">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9f5b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c9f5b-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9f5b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9f5b-144">Request</span></span>
<span data-ttu-id="c9f5b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="c9f5b-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9f5b-146">Response</span></span>
<span data-ttu-id="c9f5b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
