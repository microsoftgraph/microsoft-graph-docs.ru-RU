---
title: Применение Акцессревиев
description: 'В функции проверок доступа Azure AD примените решения завершенной Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 58fb169e3ebf71701a14cc6ad11fc32d451c78ee
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259005"
---
# <a name="apply-accessreview"></a><span data-ttu-id="77364-104">Применение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="77364-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77364-105">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD примените решения завершенной [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="77364-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="77364-106">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="77364-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="77364-107">После завершения проверки доступа либо из-за того, что она достигла даты окончания, либо администратор остановил его вручную, и автоматическое применение не настроено для проверки, вы можете вызвать Apply, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="77364-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="77364-108">Пока не будет применено, решения для удаления прав доступа не будут отображаться в исходном ресурсе, пользователи для экземпляра сохраняют сведения о членстве в группах.</span><span class="sxs-lookup"><span data-stu-id="77364-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="77364-109">Вызывая Apply, результат проверки реализуется путем обновления группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="77364-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="77364-110">Если в ходе рецензирования был запрещен доступ пользователя, то при вызове администратором этого API служба Azure AD удаляет членство или назначение приложения.</span><span class="sxs-lookup"><span data-stu-id="77364-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="77364-111">После завершения проверки доступа и автоматического применения этого параметра Состояние проверки изменится с "завершено" на "промежуточные состояния", а "наконец" изменится на "применено состояние".</span><span class="sxs-lookup"><span data-stu-id="77364-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="77364-112">Вы должны увидеть запрещенных пользователей (при их наличии), которые удаляются из назначения группы ресурсов или приложения в течение нескольких минут.</span><span class="sxs-lookup"><span data-stu-id="77364-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="77364-113">Настроенное автоматическое применение проверки или выбор применения не оказывает никакого действия для группы, созданной в локальном каталоге или в динамической группе.</span><span class="sxs-lookup"><span data-stu-id="77364-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="77364-114">Если вы хотите изменить группу, которая является локальной, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="77364-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="77364-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77364-115">Permissions</span></span>
<span data-ttu-id="77364-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77364-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77364-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77364-118">Permission type</span></span>                        | <span data-ttu-id="77364-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77364-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="77364-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77364-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="77364-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77364-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="77364-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77364-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77364-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77364-123">Not supported.</span></span> |
|<span data-ttu-id="77364-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77364-124">Application</span></span>                            | <span data-ttu-id="77364-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77364-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77364-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77364-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="77364-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77364-127">Request headers</span></span>
| <span data-ttu-id="77364-128">Имя</span><span class="sxs-lookup"><span data-stu-id="77364-128">Name</span></span>         | <span data-ttu-id="77364-129">Тип</span><span class="sxs-lookup"><span data-stu-id="77364-129">Type</span></span>        | <span data-ttu-id="77364-130">Описание</span><span class="sxs-lookup"><span data-stu-id="77364-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="77364-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="77364-131">Authorization</span></span> | <span data-ttu-id="77364-132">string</span><span class="sxs-lookup"><span data-stu-id="77364-132">string</span></span> | <span data-ttu-id="77364-p107">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77364-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77364-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77364-135">Request body</span></span>
<span data-ttu-id="77364-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77364-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="77364-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="77364-137">Response</span></span>
<span data-ttu-id="77364-p108">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77364-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="77364-140">См. также</span><span class="sxs-lookup"><span data-stu-id="77364-140">See also</span></span>

- [<span data-ttu-id="77364-141">Как выполнить проверку доступа</span><span class="sxs-lookup"><span data-stu-id="77364-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="77364-142">Пример</span><span class="sxs-lookup"><span data-stu-id="77364-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77364-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="77364-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
##### <a name="response"></a><span data-ttu-id="77364-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="77364-144">Response</span></span>
><span data-ttu-id="77364-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77364-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="77364-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="77364-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="77364-148">C#</span><span class="sxs-lookup"><span data-stu-id="77364-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/apply_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77364-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="77364-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/apply_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="77364-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77364-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/apply_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
