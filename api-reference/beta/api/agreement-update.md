---
title: Обновление соглашения
description: Обновление свойств объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ee62ae7f42c958304549883afbd66e022230bdd5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942875"
---
# <a name="update-agreement"></a><span data-ttu-id="40148-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="40148-103">Update agreement</span></span>

<span data-ttu-id="40148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40148-105">Обновление свойств объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="40148-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40148-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40148-106">Permissions</span></span>
<span data-ttu-id="40148-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40148-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40148-109">Permission type</span></span>                        | <span data-ttu-id="40148-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40148-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="40148-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40148-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40148-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40148-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="40148-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40148-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40148-114">Not supported.</span></span> |
|<span data-ttu-id="40148-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40148-115">Application</span></span>                            | <span data-ttu-id="40148-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40148-116">Not supported.</span></span> |

<span data-ttu-id="40148-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="40148-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="40148-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="40148-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="40148-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="40148-119">Global Administrator</span></span>
+ <span data-ttu-id="40148-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="40148-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="40148-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="40148-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="40148-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40148-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40148-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40148-123">Request headers</span></span>
| <span data-ttu-id="40148-124">Имя</span><span class="sxs-lookup"><span data-stu-id="40148-124">Name</span></span>         | <span data-ttu-id="40148-125">Тип</span><span class="sxs-lookup"><span data-stu-id="40148-125">Type</span></span>        | <span data-ttu-id="40148-126">Описание</span><span class="sxs-lookup"><span data-stu-id="40148-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="40148-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="40148-127">Authorization</span></span> | <span data-ttu-id="40148-128">string</span><span class="sxs-lookup"><span data-stu-id="40148-128">string</span></span> | <span data-ttu-id="40148-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40148-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40148-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40148-131">Request body</span></span>
<span data-ttu-id="40148-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="40148-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="40148-133">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="40148-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="40148-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="40148-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40148-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="40148-135">Property</span></span>     | <span data-ttu-id="40148-136">Тип</span><span class="sxs-lookup"><span data-stu-id="40148-136">Type</span></span>        | <span data-ttu-id="40148-137">Описание</span><span class="sxs-lookup"><span data-stu-id="40148-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40148-138">displayName</span><span class="sxs-lookup"><span data-stu-id="40148-138">displayName</span></span>|<span data-ttu-id="40148-139">Строка</span><span class="sxs-lookup"><span data-stu-id="40148-139">String</span></span>|<span data-ttu-id="40148-140">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="40148-140">Display name of the agreement.</span></span>|
|<span data-ttu-id="40148-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="40148-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="40148-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="40148-142">Boolean</span></span>|<span data-ttu-id="40148-143">Необходимо ли пользователю расширить и просмотреть соглашение перед его принятием.</span><span class="sxs-lookup"><span data-stu-id="40148-143">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="40148-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="40148-144">Response</span></span>
<span data-ttu-id="40148-145">В случае успешной работы этот метод возвращает код отклика и обновленный объект соглашения `200 OK` в тексте [](../resources/agreement.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="40148-145">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40148-146">Пример</span><span class="sxs-lookup"><span data-stu-id="40148-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40148-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="40148-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="40148-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="40148-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40148-149">C#</span><span class="sxs-lookup"><span data-stu-id="40148-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40148-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40148-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40148-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40148-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40148-152">Java</span><span class="sxs-lookup"><span data-stu-id="40148-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40148-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="40148-153">Response</span></span>
><span data-ttu-id="40148-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40148-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


