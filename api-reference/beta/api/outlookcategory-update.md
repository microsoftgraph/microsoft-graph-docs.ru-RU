---
title: Обновление категории Outlook
description: 'Обновление перезаписываемого свойства **color** указанного объекта outlookCategory. Не удается изменить свойство **displayName** '
ms.openlocfilehash: c9dee74de9955495e0134f68d00a75929a46f16e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079034"
---
# <a name="update-outlook-category"></a><span data-ttu-id="5b72b-104">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="5b72b-104">Update Outlook category</span></span>

> <span data-ttu-id="5b72b-105">**Важно**: интерфейсы API в разделе версии /beta в Microsoft Graph в предварительной версии и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b72b-105">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b72b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b72b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b72b-107">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="5b72b-107">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="5b72b-108">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="5b72b-108">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b72b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b72b-109">Permissions</span></span>
<span data-ttu-id="5b72b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b72b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b72b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b72b-112">Permission type</span></span>      | <span data-ttu-id="5b72b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b72b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b72b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b72b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5b72b-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b72b-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5b72b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b72b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b72b-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b72b-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5b72b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b72b-118">Application</span></span> | <span data-ttu-id="5b72b-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b72b-119">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b72b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b72b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b72b-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b72b-121">Optional query parameters</span></span>
<span data-ttu-id="5b72b-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b72b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b72b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b72b-123">Request headers</span></span>
| <span data-ttu-id="5b72b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5b72b-124">Name</span></span>      |<span data-ttu-id="5b72b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5b72b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b72b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b72b-126">Authorization</span></span>  | <span data-ttu-id="5b72b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b72b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b72b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b72b-129">Request body</span></span>
<span data-ttu-id="5b72b-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5b72b-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5b72b-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b72b-133">Property</span></span>     | <span data-ttu-id="5b72b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5b72b-134">Type</span></span>   |<span data-ttu-id="5b72b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5b72b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b72b-136">color</span><span class="sxs-lookup"><span data-stu-id="5b72b-136">color</span></span>|<span data-ttu-id="5b72b-137">String</span><span class="sxs-lookup"><span data-stu-id="5b72b-137">String</span></span>|<span data-ttu-id="5b72b-138">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="5b72b-138">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="5b72b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b72b-139">Response</span></span>

<span data-ttu-id="5b72b-140">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b72b-140">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b72b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5b72b-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b72b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b72b-142">Request</span></span>
<span data-ttu-id="5b72b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b72b-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="5b72b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b72b-144">Response</span></span>
<span data-ttu-id="5b72b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5b72b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->