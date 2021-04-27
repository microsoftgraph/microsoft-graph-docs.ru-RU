---
title: Применение accessReview
description: 'В функции обзоров доступа Azure AD применяются решения завершенного accessReview.  Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b590b741915aaf9ef901ee51e2eb11d43f9b439f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048535"
---
# <a name="apply-accessreview"></a><span data-ttu-id="847d9-104">Применение accessReview</span><span class="sxs-lookup"><span data-stu-id="847d9-104">Apply accessReview</span></span>

<span data-ttu-id="847d9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="847d9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="847d9-106">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) применяются решения завершенного [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="847d9-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="847d9-107">Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="847d9-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="847d9-108">После завершения проверки доступа, либо из-за того, что он достиг конечной даты, либо администратор остановил его вручную, а автоматическое применение не было настроено для проверки, можно вызвать Apply, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="847d9-108">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="847d9-109">Пока не применяется, решения об устранении прав доступа не отображаются на исходный ресурс, например, пользователи сохраняют свои групповые членства.</span><span class="sxs-lookup"><span data-stu-id="847d9-109">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="847d9-110">При вызове применяются результаты проверки, обновляя группу или приложение.</span><span class="sxs-lookup"><span data-stu-id="847d9-110">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="847d9-111">Если в обзоре пользователю было отказано в доступе, при вызове администратором этого API Azure AD удаляет назначение членства или приложения.</span><span class="sxs-lookup"><span data-stu-id="847d9-111">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="847d9-112">После завершения проверки доступа и настройки автоматического применения состояние обзора будет изменяться с Завершено на промежуточные состояния и, наконец, изменится на состояние Applied.</span><span class="sxs-lookup"><span data-stu-id="847d9-112">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="847d9-113">Ожидается, что в течение нескольких минут пользователи будут удалены из группы ресурсов или назначения приложений.</span><span class="sxs-lookup"><span data-stu-id="847d9-113">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="847d9-114">Настроенный обзор автоматического применения или выбор Apply не влияют на группу, которая возникает в локальном каталоге или динамической группе.</span><span class="sxs-lookup"><span data-stu-id="847d9-114">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="847d9-115">Если вы хотите изменить группу, которая создается локально, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="847d9-115">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="847d9-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="847d9-116">Permissions</span></span>
<span data-ttu-id="847d9-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="847d9-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="847d9-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="847d9-119">Permission type</span></span>                        | <span data-ttu-id="847d9-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="847d9-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="847d9-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="847d9-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="847d9-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847d9-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="847d9-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="847d9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="847d9-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847d9-124">Not supported.</span></span> |
|<span data-ttu-id="847d9-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="847d9-125">Application</span></span>                            | <span data-ttu-id="847d9-126">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="847d9-126">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="847d9-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="847d9-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a><span data-ttu-id="847d9-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="847d9-128">Request headers</span></span>
| <span data-ttu-id="847d9-129">Имя</span><span class="sxs-lookup"><span data-stu-id="847d9-129">Name</span></span>         | <span data-ttu-id="847d9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="847d9-130">Type</span></span>        | <span data-ttu-id="847d9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="847d9-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="847d9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="847d9-132">Authorization</span></span> | <span data-ttu-id="847d9-133">string</span><span class="sxs-lookup"><span data-stu-id="847d9-133">string</span></span> | <span data-ttu-id="847d9-p107">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="847d9-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="847d9-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="847d9-136">Request body</span></span>
<span data-ttu-id="847d9-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="847d9-137">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="847d9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="847d9-138">Response</span></span>
<span data-ttu-id="847d9-p108">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="847d9-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="847d9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="847d9-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="847d9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="847d9-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="847d9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="847d9-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="847d9-144">C#</span><span class="sxs-lookup"><span data-stu-id="847d9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="847d9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="847d9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="847d9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="847d9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="847d9-147">Java</span><span class="sxs-lookup"><span data-stu-id="847d9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="847d9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="847d9-148">Response</span></span>
><span data-ttu-id="847d9-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="847d9-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="847d9-150">См. также</span><span class="sxs-lookup"><span data-stu-id="847d9-150">See also</span></span>

- [<span data-ttu-id="847d9-151">Завершение проверки доступа</span><span class="sxs-lookup"><span data-stu-id="847d9-151">How to complete an access review</span></span>](/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)
