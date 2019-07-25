---
title: Обновление соглашения
description: Обновление свойств объекта договора.
localization_priority: Normal
ms.openlocfilehash: d50f271845077b26b135d1211ee13f365d812e8c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855499"
---
# <a name="update-agreement"></a><span data-ttu-id="c9b56-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="c9b56-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b56-104">Обновление свойств объекта [договора](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="c9b56-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9b56-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b56-105">Permissions</span></span>
<span data-ttu-id="c9b56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b56-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b56-108">Permission type</span></span>                        | <span data-ttu-id="c9b56-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9b56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9b56-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9b56-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9b56-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b56-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="c9b56-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9b56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9b56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b56-113">Not supported.</span></span> |
|<span data-ttu-id="c9b56-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9b56-114">Application</span></span>                            | <span data-ttu-id="c9b56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9b56-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9b56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="c9b56-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9b56-117">Request headers</span></span>
| <span data-ttu-id="c9b56-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c9b56-118">Name</span></span>         | <span data-ttu-id="c9b56-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c9b56-119">Type</span></span>        | <span data-ttu-id="c9b56-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9b56-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c9b56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b56-121">Authorization</span></span> | <span data-ttu-id="c9b56-122">string</span><span class="sxs-lookup"><span data-stu-id="c9b56-122">string</span></span> | <span data-ttu-id="c9b56-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9b56-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9b56-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9b56-125">Request body</span></span>
<span data-ttu-id="c9b56-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c9b56-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c9b56-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c9b56-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c9b56-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c9b56-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9b56-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9b56-129">Property</span></span>     | <span data-ttu-id="c9b56-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9b56-130">Type</span></span>        | <span data-ttu-id="c9b56-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9b56-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9b56-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c9b56-132">displayName</span></span>|<span data-ttu-id="c9b56-133">String</span><span class="sxs-lookup"><span data-stu-id="c9b56-133">String</span></span>|<span data-ttu-id="c9b56-134">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="c9b56-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="c9b56-135">Исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="c9b56-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="c9b56-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b56-136">Boolean</span></span>|<span data-ttu-id="c9b56-137">Следует ли пользователю разворачивать и просматривать соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="c9b56-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="c9b56-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b56-138">Response</span></span>
<span data-ttu-id="c9b56-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9b56-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9b56-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c9b56-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9b56-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9b56-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9b56-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9b56-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9b56-143">C#</span><span class="sxs-lookup"><span data-stu-id="c9b56-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9b56-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9b56-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9b56-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9b56-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9b56-146">Java</span><span class="sxs-lookup"><span data-stu-id="c9b56-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9b56-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b56-147">Response</span></span>
><span data-ttu-id="c9b56-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9b56-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
