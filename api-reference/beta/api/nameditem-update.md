---
title: Обновление объекта NamedItem
description: Обновление свойств объекта nameditem.
localization_priority: Normal
ms.openlocfilehash: ffb01e0998b3b94706e50ed461014fcfd11ce927
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514049"
---
# <a name="update-nameditem"></a><span data-ttu-id="2173f-103">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="2173f-103">Update nameditem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2173f-104">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="2173f-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2173f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2173f-105">Permissions</span></span>
<span data-ttu-id="2173f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2173f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2173f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2173f-108">Permission type</span></span>      | <span data-ttu-id="2173f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2173f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2173f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2173f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2173f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2173f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2173f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2173f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2173f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2173f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2173f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2173f-114">Application</span></span> | <span data-ttu-id="2173f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2173f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2173f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2173f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="2173f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2173f-117">Optional request headers</span></span>
| <span data-ttu-id="2173f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2173f-118">Name</span></span>       | <span data-ttu-id="2173f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2173f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2173f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2173f-120">Authorization</span></span>  | <span data-ttu-id="2173f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2173f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2173f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2173f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2173f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2173f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2173f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2173f-126">Request body</span></span>
<span data-ttu-id="2173f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2173f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2173f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2173f-130">Property</span></span>     | <span data-ttu-id="2173f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2173f-131">Type</span></span>   |<span data-ttu-id="2173f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2173f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2173f-133">visible</span><span class="sxs-lookup"><span data-stu-id="2173f-133">visible</span></span>|<span data-ttu-id="2173f-134">boolean</span><span class="sxs-lookup"><span data-stu-id="2173f-134">boolean</span></span>|<span data-ttu-id="2173f-135">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="2173f-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="2173f-136">comment</span><span class="sxs-lookup"><span data-stu-id="2173f-136">comment</span></span>|   <span data-ttu-id="2173f-137">строка</span><span class="sxs-lookup"><span data-stu-id="2173f-137">string</span></span>  |<span data-ttu-id="2173f-138">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="2173f-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="2173f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2173f-139">Response</span></span>

<span data-ttu-id="2173f-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2173f-140">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2173f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2173f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2173f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2173f-142">Request</span></span>
<span data-ttu-id="2173f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2173f-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2173f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2173f-144">Response</span></span>
<span data-ttu-id="2173f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2173f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
