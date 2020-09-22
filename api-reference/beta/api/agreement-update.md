---
title: Обновление соглашения
description: Обновление свойств объекта договора.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 07b8fce1de78ac062ae9ea38ed4d22a5d345cace
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997139"
---
# <a name="update-agreement"></a><span data-ttu-id="c9d0e-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="c9d0e-103">Update agreement</span></span>

<span data-ttu-id="c9d0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d0e-105">Обновление свойств объекта [договора](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="c9d0e-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9d0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d0e-106">Permissions</span></span>
<span data-ttu-id="c9d0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d0e-109">Permission type</span></span>                        | <span data-ttu-id="c9d0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9d0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9d0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9d0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9d0e-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d0e-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="c9d0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9d0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9d0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-114">Not supported.</span></span> |
|<span data-ttu-id="c9d0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9d0e-115">Application</span></span>                            | <span data-ttu-id="c9d0e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9d0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9d0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c9d0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9d0e-118">Request headers</span></span>
| <span data-ttu-id="c9d0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c9d0e-119">Name</span></span>         | <span data-ttu-id="c9d0e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c9d0e-120">Type</span></span>        | <span data-ttu-id="c9d0e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c9d0e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c9d0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9d0e-122">Authorization</span></span> | <span data-ttu-id="c9d0e-123">string</span><span class="sxs-lookup"><span data-stu-id="c9d0e-123">string</span></span> | <span data-ttu-id="c9d0e-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9d0e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9d0e-126">Request body</span></span>
<span data-ttu-id="c9d0e-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c9d0e-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c9d0e-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9d0e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9d0e-130">Property</span></span>     | <span data-ttu-id="c9d0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9d0e-131">Type</span></span>        | <span data-ttu-id="c9d0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9d0e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9d0e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c9d0e-133">displayName</span></span>|<span data-ttu-id="c9d0e-134">String</span><span class="sxs-lookup"><span data-stu-id="c9d0e-134">String</span></span>|<span data-ttu-id="c9d0e-135">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="c9d0e-136">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="c9d0e-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="c9d0e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d0e-137">Boolean</span></span>|<span data-ttu-id="c9d0e-138">Следует ли пользователю разворачивать и просматривать соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="c9d0e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d0e-139">Response</span></span>
<span data-ttu-id="c9d0e-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9d0e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c9d0e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9d0e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9d0e-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c9d0e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d0e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="c9d0e-144">C#</span><span class="sxs-lookup"><span data-stu-id="c9d0e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9d0e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9d0e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9d0e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9d0e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9d0e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d0e-147">Response</span></span>
><span data-ttu-id="c9d0e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9d0e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


