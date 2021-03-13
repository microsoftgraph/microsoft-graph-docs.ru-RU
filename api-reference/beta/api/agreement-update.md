---
title: Обновление соглашения
description: Обновление свойств объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 88bab29854bd474221df81241698b57fa94be79a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773930"
---
# <a name="update-agreement"></a><span data-ttu-id="2d814-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="2d814-103">Update agreement</span></span>

<span data-ttu-id="2d814-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d814-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d814-105">Обновление свойств объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="2d814-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d814-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d814-106">Permissions</span></span>
<span data-ttu-id="2d814-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d814-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d814-109">Permission type</span></span>                        | <span data-ttu-id="2d814-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d814-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d814-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d814-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d814-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d814-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="2d814-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d814-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d814-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d814-114">Not supported.</span></span> |
|<span data-ttu-id="2d814-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d814-115">Application</span></span>                            | <span data-ttu-id="2d814-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d814-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d814-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d814-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2d814-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d814-118">Request headers</span></span>
| <span data-ttu-id="2d814-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2d814-119">Name</span></span>         | <span data-ttu-id="2d814-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2d814-120">Type</span></span>        | <span data-ttu-id="2d814-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2d814-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2d814-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d814-122">Authorization</span></span> | <span data-ttu-id="2d814-123">string</span><span class="sxs-lookup"><span data-stu-id="2d814-123">string</span></span> | <span data-ttu-id="2d814-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d814-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d814-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d814-126">Request body</span></span>
<span data-ttu-id="2d814-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2d814-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2d814-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2d814-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d814-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2d814-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d814-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d814-130">Property</span></span>     | <span data-ttu-id="2d814-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d814-131">Type</span></span>        | <span data-ttu-id="2d814-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d814-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d814-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2d814-133">displayName</span></span>|<span data-ttu-id="2d814-134">String</span><span class="sxs-lookup"><span data-stu-id="2d814-134">String</span></span>|<span data-ttu-id="2d814-135">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="2d814-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="2d814-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="2d814-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="2d814-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d814-137">Boolean</span></span>|<span data-ttu-id="2d814-138">Необходимо ли пользователю расширить и просмотреть соглашение перед его принятием.</span><span class="sxs-lookup"><span data-stu-id="2d814-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="2d814-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d814-139">Response</span></span>
<span data-ttu-id="2d814-140">В случае успешной работы этот метод возвращает код отклика и обновленный объект соглашения `200 OK` в тексте [](../resources/agreement.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="2d814-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d814-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2d814-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d814-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d814-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2d814-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d814-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="2d814-144">C#</span><span class="sxs-lookup"><span data-stu-id="2d814-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d814-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d814-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d814-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d814-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d814-147">Java</span><span class="sxs-lookup"><span data-stu-id="2d814-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d814-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d814-148">Response</span></span>
><span data-ttu-id="2d814-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d814-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


