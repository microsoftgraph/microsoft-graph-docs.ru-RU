---
title: Обновление соглашения
description: Обновление свойств объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 77c3fbf6aa37d283e02408a1000d4a5f521a3fd5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048199"
---
# <a name="update-agreement"></a><span data-ttu-id="1d72c-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="1d72c-103">Update agreement</span></span>

<span data-ttu-id="1d72c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d72c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d72c-105">Обновление свойств объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="1d72c-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d72c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d72c-106">Permissions</span></span>
<span data-ttu-id="1d72c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d72c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d72c-109">Permission type</span></span>                        | <span data-ttu-id="1d72c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d72c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d72c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d72c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d72c-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d72c-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="1d72c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d72c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d72c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d72c-114">Not supported.</span></span> |
|<span data-ttu-id="1d72c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d72c-115">Application</span></span>                            | <span data-ttu-id="1d72c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d72c-116">Not supported.</span></span> |

<span data-ttu-id="1d72c-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="1d72c-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="1d72c-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="1d72c-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="1d72c-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1d72c-119">Global Administrator</span></span>
+ <span data-ttu-id="1d72c-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="1d72c-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="1d72c-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="1d72c-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1d72c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d72c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1d72c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d72c-123">Request headers</span></span>
| <span data-ttu-id="1d72c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1d72c-124">Name</span></span>         | <span data-ttu-id="1d72c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="1d72c-125">Type</span></span>        | <span data-ttu-id="1d72c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1d72c-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1d72c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d72c-127">Authorization</span></span> | <span data-ttu-id="1d72c-128">string</span><span class="sxs-lookup"><span data-stu-id="1d72c-128">string</span></span> | <span data-ttu-id="1d72c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d72c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d72c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d72c-131">Request body</span></span>
<span data-ttu-id="1d72c-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1d72c-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1d72c-133">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1d72c-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1d72c-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1d72c-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d72c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d72c-135">Property</span></span>     | <span data-ttu-id="1d72c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="1d72c-136">Type</span></span>        | <span data-ttu-id="1d72c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="1d72c-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d72c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1d72c-138">displayName</span></span>|<span data-ttu-id="1d72c-139">String</span><span class="sxs-lookup"><span data-stu-id="1d72c-139">String</span></span>|<span data-ttu-id="1d72c-140">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="1d72c-140">Display name of the agreement.</span></span>|
|<span data-ttu-id="1d72c-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="1d72c-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1d72c-142">Логический</span><span class="sxs-lookup"><span data-stu-id="1d72c-142">Boolean</span></span>|<span data-ttu-id="1d72c-143">Необходимо ли пользователю расширить и просмотреть соглашение перед его принятием.</span><span class="sxs-lookup"><span data-stu-id="1d72c-143">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="1d72c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d72c-144">Response</span></span>
<span data-ttu-id="1d72c-145">В случае успешной работы этот метод возвращает код отклика и обновленный объект соглашения `200 OK` в тексте [](../resources/agreement.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="1d72c-145">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d72c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="1d72c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d72c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d72c-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1d72c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d72c-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1d72c-149">C#</span><span class="sxs-lookup"><span data-stu-id="1d72c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d72c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d72c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d72c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d72c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d72c-152">Java</span><span class="sxs-lookup"><span data-stu-id="1d72c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d72c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d72c-153">Response</span></span>
><span data-ttu-id="1d72c-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d72c-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


