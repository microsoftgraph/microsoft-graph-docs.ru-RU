---
title: Обновление категории Outlook
description: 'Обновление перезаписываемого свойства **color** указанного объекта outlookCategory. Не удается изменить свойство **displayName** '
ms.openlocfilehash: 1b664ef4414a798fe3f8ee2cd517a75f96ff3dc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028237"
---
# <a name="update-outlook-category"></a><span data-ttu-id="2efe4-104">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="2efe4-104">Update Outlook category</span></span>


<span data-ttu-id="2efe4-105">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="2efe4-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="2efe4-106">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="2efe4-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="2efe4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2efe4-107">Permissions</span></span>
<span data-ttu-id="2efe4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2efe4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2efe4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2efe4-110">Permission type</span></span>      | <span data-ttu-id="2efe4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2efe4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2efe4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2efe4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2efe4-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2efe4-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="2efe4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2efe4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2efe4-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2efe4-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="2efe4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2efe4-116">Application</span></span> | <span data-ttu-id="2efe4-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2efe4-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2efe4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2efe4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2efe4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2efe4-119">Optional query parameters</span></span>
<span data-ttu-id="2efe4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2efe4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2efe4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2efe4-121">Request headers</span></span>
| <span data-ttu-id="2efe4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2efe4-122">Name</span></span>      |<span data-ttu-id="2efe4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2efe4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2efe4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2efe4-124">Authorization</span></span>  | <span data-ttu-id="2efe4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2efe4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2efe4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2efe4-127">Request body</span></span>
<span data-ttu-id="2efe4-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2efe4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2efe4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2efe4-131">Property</span></span>     | <span data-ttu-id="2efe4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2efe4-132">Type</span></span>   |<span data-ttu-id="2efe4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2efe4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2efe4-134">color</span><span class="sxs-lookup"><span data-stu-id="2efe4-134">color</span></span>|<span data-ttu-id="2efe4-135">String</span><span class="sxs-lookup"><span data-stu-id="2efe4-135">String</span></span>|<span data-ttu-id="2efe4-136">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="2efe4-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="2efe4-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="2efe4-137">Response</span></span>

<span data-ttu-id="2efe4-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2efe4-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2efe4-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2efe4-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2efe4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2efe4-140">Request</span></span>
<span data-ttu-id="2efe4-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2efe4-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="2efe4-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="2efe4-142">Response</span></span>
<span data-ttu-id="2efe4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2efe4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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