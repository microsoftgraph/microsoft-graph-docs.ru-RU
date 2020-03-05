---
title: Применение Акцессревиев
description: 'В функции проверок доступа Azure AD примените решения завершенной Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd24db15accc6a969097504224166f13a19f3865
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441923"
---
# <a name="apply-accessreview"></a><span data-ttu-id="9f0b1-104">Применение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="9f0b1-104">Apply accessReview</span></span>

<span data-ttu-id="9f0b1-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f0b1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f0b1-106">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD примените решения завершенной [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="9f0b1-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="9f0b1-107">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="9f0b1-108">После завершения проверки доступа либо из-за того, что она достигла даты окончания, либо администратор остановил его вручную, и автоматическое применение не настроено для проверки, вы можете вызвать Apply, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-108">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="9f0b1-109">Пока не будет применено, решения для удаления прав доступа не будут отображаться в исходном ресурсе, пользователи для экземпляра сохраняют сведения о членстве в группах.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-109">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="9f0b1-110">Вызывая Apply, результат проверки реализуется путем обновления группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-110">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="9f0b1-111">Если в ходе рецензирования был запрещен доступ пользователя, то при вызове администратором этого API служба Azure AD удаляет членство или назначение приложения.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-111">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="9f0b1-112">После завершения проверки доступа и автоматического применения этого параметра Состояние проверки изменится с "завершено" на "промежуточные состояния", а "наконец" изменится на "применено состояние".</span><span class="sxs-lookup"><span data-stu-id="9f0b1-112">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="9f0b1-113">Вы должны увидеть запрещенных пользователей (при их наличии), которые удаляются из назначения группы ресурсов или приложения в течение нескольких минут.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-113">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="9f0b1-114">Настроенное автоматическое применение проверки или выбор применения не оказывает никакого действия для группы, созданной в локальном каталоге или в динамической группе.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-114">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="9f0b1-115">Если вы хотите изменить группу, которая является локальной, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-115">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="9f0b1-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f0b1-116">Permissions</span></span>
<span data-ttu-id="9f0b1-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f0b1-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f0b1-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f0b1-119">Permission type</span></span>                        | <span data-ttu-id="9f0b1-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f0b1-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f0b1-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f0b1-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f0b1-122">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9f0b1-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9f0b1-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f0b1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f0b1-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-124">Not supported.</span></span> |
|<span data-ttu-id="9f0b1-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f0b1-125">Application</span></span>                            | <span data-ttu-id="9f0b1-126">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="9f0b1-126">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f0b1-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f0b1-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a><span data-ttu-id="9f0b1-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f0b1-128">Request headers</span></span>
| <span data-ttu-id="9f0b1-129">Имя</span><span class="sxs-lookup"><span data-stu-id="9f0b1-129">Name</span></span>         | <span data-ttu-id="9f0b1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f0b1-130">Type</span></span>        | <span data-ttu-id="9f0b1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f0b1-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9f0b1-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f0b1-132">Authorization</span></span> | <span data-ttu-id="9f0b1-133">string</span><span class="sxs-lookup"><span data-stu-id="9f0b1-133">string</span></span> | <span data-ttu-id="9f0b1-p107">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f0b1-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f0b1-136">Request body</span></span>
<span data-ttu-id="9f0b1-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-137">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9f0b1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f0b1-138">Response</span></span>
<span data-ttu-id="9f0b1-p108">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="9f0b1-141">См. также</span><span class="sxs-lookup"><span data-stu-id="9f0b1-141">See also</span></span>

- [<span data-ttu-id="9f0b1-142">Как выполнить проверку доступа</span><span class="sxs-lookup"><span data-stu-id="9f0b1-142">How to complete an access review</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="9f0b1-143">Пример</span><span class="sxs-lookup"><span data-stu-id="9f0b1-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f0b1-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f0b1-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9f0b1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f0b1-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="9f0b1-146">C#</span><span class="sxs-lookup"><span data-stu-id="9f0b1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f0b1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f0b1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f0b1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f0b1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f0b1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f0b1-149">Response</span></span>
><span data-ttu-id="9f0b1-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f0b1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
