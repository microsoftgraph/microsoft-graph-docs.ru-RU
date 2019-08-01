---
title: Применение Акцессревиев
description: 'В функции проверок доступа Azure AD примените решения завершенной Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a1affb6af03a60bd2b9c164254e0ae4a9bf4f43
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049535"
---
# <a name="apply-accessreview"></a><span data-ttu-id="148d2-104">Применение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="148d2-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="148d2-105">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD примените решения завершенной [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="148d2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="148d2-106">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="148d2-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="148d2-107">После завершения проверки доступа либо из-за того, что она достигла даты окончания, либо администратор остановил его вручную, и автоматическое применение не настроено для проверки, вы можете вызвать Apply, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="148d2-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="148d2-108">Пока не будет применено, решения для удаления прав доступа не будут отображаться в исходном ресурсе, пользователи для экземпляра сохраняют сведения о членстве в группах.</span><span class="sxs-lookup"><span data-stu-id="148d2-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="148d2-109">Вызывая Apply, результат проверки реализуется путем обновления группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="148d2-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="148d2-110">Если в ходе рецензирования был запрещен доступ пользователя, то при вызове администратором этого API служба Azure AD удаляет членство или назначение приложения.</span><span class="sxs-lookup"><span data-stu-id="148d2-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="148d2-111">После завершения проверки доступа и автоматического применения этого параметра Состояние проверки изменится с "завершено" на "промежуточные состояния", а "наконец" изменится на "применено состояние".</span><span class="sxs-lookup"><span data-stu-id="148d2-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="148d2-112">Вы должны увидеть запрещенных пользователей (при их наличии), которые удаляются из назначения группы ресурсов или приложения в течение нескольких минут.</span><span class="sxs-lookup"><span data-stu-id="148d2-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="148d2-113">Настроенное автоматическое применение проверки или выбор применения не оказывает никакого действия для группы, созданной в локальном каталоге или в динамической группе.</span><span class="sxs-lookup"><span data-stu-id="148d2-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="148d2-114">Если вы хотите изменить группу, которая является локальной, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="148d2-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="148d2-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="148d2-115">Permissions</span></span>
<span data-ttu-id="148d2-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="148d2-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148d2-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="148d2-118">Permission type</span></span>                        | <span data-ttu-id="148d2-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="148d2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="148d2-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="148d2-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="148d2-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148d2-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="148d2-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="148d2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="148d2-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="148d2-123">Not supported.</span></span> |
|<span data-ttu-id="148d2-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="148d2-124">Application</span></span>                            | <span data-ttu-id="148d2-125">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="148d2-125">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="148d2-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="148d2-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="148d2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="148d2-127">Request headers</span></span>
| <span data-ttu-id="148d2-128">Имя</span><span class="sxs-lookup"><span data-stu-id="148d2-128">Name</span></span>         | <span data-ttu-id="148d2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="148d2-129">Type</span></span>        | <span data-ttu-id="148d2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="148d2-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="148d2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="148d2-131">Authorization</span></span> | <span data-ttu-id="148d2-132">string</span><span class="sxs-lookup"><span data-stu-id="148d2-132">string</span></span> | <span data-ttu-id="148d2-p107">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="148d2-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="148d2-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="148d2-135">Request body</span></span>
<span data-ttu-id="148d2-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="148d2-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="148d2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="148d2-137">Response</span></span>
<span data-ttu-id="148d2-p108">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="148d2-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="148d2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="148d2-140">See also</span></span>

- [<span data-ttu-id="148d2-141">Как выполнить проверку доступа</span><span class="sxs-lookup"><span data-stu-id="148d2-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="148d2-142">Пример</span><span class="sxs-lookup"><span data-stu-id="148d2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="148d2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="148d2-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="148d2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="148d2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="148d2-145">C#</span><span class="sxs-lookup"><span data-stu-id="148d2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="148d2-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="148d2-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="148d2-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="148d2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="148d2-148">Java</span><span class="sxs-lookup"><span data-stu-id="148d2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="148d2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="148d2-149">Response</span></span>
><span data-ttu-id="148d2-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="148d2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
