---
title: Обновление соглашения
description: Обновление свойств объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 53ec2db520eb6933526753c8326f6a4d2ee95f34
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774942"
---
# <a name="update-agreement"></a><span data-ttu-id="9ce3b-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="9ce3b-103">Update agreement</span></span>

<span data-ttu-id="9ce3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ce3b-105">Обновление свойств объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="9ce3b-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ce3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce3b-106">Permissions</span></span>
<span data-ttu-id="9ce3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce3b-109">Permission type</span></span>                        | <span data-ttu-id="9ce3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ce3b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ce3b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ce3b-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce3b-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9ce3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ce3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ce3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-114">Not supported.</span></span> |
|<span data-ttu-id="9ce3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ce3b-115">Application</span></span>                            | <span data-ttu-id="9ce3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ce3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ce3b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9ce3b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ce3b-118">Request headers</span></span>
| <span data-ttu-id="9ce3b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9ce3b-119">Name</span></span>         | <span data-ttu-id="9ce3b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce3b-120">Type</span></span>        | <span data-ttu-id="9ce3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce3b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ce3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce3b-122">Authorization</span></span> | <span data-ttu-id="9ce3b-123">string</span><span class="sxs-lookup"><span data-stu-id="9ce3b-123">string</span></span> | <span data-ttu-id="9ce3b-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ce3b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ce3b-126">Request body</span></span>
<span data-ttu-id="9ce3b-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9ce3b-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9ce3b-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="9ce3b-130">Для обновления поддерживаются только следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-130">Only the following properties are supported for update.</span></span>

| <span data-ttu-id="9ce3b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ce3b-131">Property</span></span>     | <span data-ttu-id="9ce3b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce3b-132">Type</span></span>        | <span data-ttu-id="9ce3b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce3b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ce3b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce3b-134">displayName</span></span>|<span data-ttu-id="9ce3b-135">String</span><span class="sxs-lookup"><span data-stu-id="9ce3b-135">String</span></span>|<span data-ttu-id="9ce3b-136">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="9ce3b-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="9ce3b-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="9ce3b-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ce3b-138">Boolean</span></span>|<span data-ttu-id="9ce3b-139">Необходимо ли пользователю расширить и просмотреть соглашение перед его принятием.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="9ce3b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce3b-140">Response</span></span>
<span data-ttu-id="9ce3b-141">В случае успешной работы этот метод возвращает код отклика и обновленный объект соглашения `200 OK` в тексте [](../resources/agreement.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ce3b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9ce3b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ce3b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce3b-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9ce3b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce3b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
Content-type: application/json
Content-length: 85

{
  "displayName": "Sample ToU display name",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="9ce3b-145">C#</span><span class="sxs-lookup"><span data-stu-id="9ce3b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce3b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce3b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce3b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce3b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ce3b-148">Java</span><span class="sxs-lookup"><span data-stu-id="9ce3b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ce3b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce3b-149">Response</span></span>
><span data-ttu-id="9ce3b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce3b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "displayName": "Sample ToU display name",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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


