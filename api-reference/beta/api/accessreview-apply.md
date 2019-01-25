---
title: Применение accessReview
description: 'В Azure AD доступ к функции проверки, применение решения завершенных accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512215"
---
# <a name="apply-accessreview"></a><span data-ttu-id="e04a2-104">Применение accessReview</span><span class="sxs-lookup"><span data-stu-id="e04a2-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e04a2-105">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD применение решения завершенных [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="e04a2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="e04a2-106">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="e04a2-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="e04a2-107">После завершения проверки доступа, либо так, как связаться с вами дату окончания или администратор остановлена вручную и автоматически назначаемой не был настроен на проверку, можно вызвать применить, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="e04a2-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="e04a2-108">Пока не происходит применить о решениях для удаления права доступа не отображаются на ресурсов источника, пользователей, например сохранять их членства в группе.</span><span class="sxs-lookup"><span data-stu-id="e04a2-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="e04a2-109">Путем вызова применения, результат проверки реализована путем обновления группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="e04a2-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="e04a2-110">Если нет доступа пользователя в разделе review, когда администратор вызывает этот интерфейс API, Azure AD удалит их назначения членства или приложения.</span><span class="sxs-lookup"><span data-stu-id="e04a2-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="e04a2-111">После проверки доступа по завершении работы и автоматически назначаемой был настроен, то состояние проверки будет заменен завершено промежуточного состояния и наконец изменится на состояние применения.</span><span class="sxs-lookup"><span data-stu-id="e04a2-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="e04a2-112">При любой, удаляемого из ресурса групповой членства или приложение назначения всего за несколько минут должно привести для просмотра запрещенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="e04a2-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="e04a2-113">Настроенные автоматическое применение проверки или выбор применить не влияет на группы, которая исходит в локальном каталоге или динамические группы.</span><span class="sxs-lookup"><span data-stu-id="e04a2-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="e04a2-114">Если вы хотите изменить группу, которая исходит локальной, загрузите результаты и применить эти изменения к представление группы в этой папке.</span><span class="sxs-lookup"><span data-stu-id="e04a2-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="e04a2-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e04a2-115">Permissions</span></span>
<span data-ttu-id="e04a2-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e04a2-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e04a2-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e04a2-118">Permission type</span></span>                        | <span data-ttu-id="e04a2-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e04a2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e04a2-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e04a2-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="e04a2-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04a2-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e04a2-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e04a2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e04a2-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e04a2-123">Not supported.</span></span> |
|<span data-ttu-id="e04a2-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e04a2-124">Application</span></span>                            | <span data-ttu-id="e04a2-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e04a2-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e04a2-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e04a2-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="e04a2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e04a2-127">Request headers</span></span>
| <span data-ttu-id="e04a2-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e04a2-128">Name</span></span>         | <span data-ttu-id="e04a2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e04a2-129">Type</span></span>        | <span data-ttu-id="e04a2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e04a2-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e04a2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e04a2-131">Authorization</span></span> | <span data-ttu-id="e04a2-132">string</span><span class="sxs-lookup"><span data-stu-id="e04a2-132">string</span></span> | <span data-ttu-id="e04a2-133">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="e04a2-133">Bearer \{token\}.</span></span> <span data-ttu-id="e04a2-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e04a2-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e04a2-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e04a2-135">Request body</span></span>
<span data-ttu-id="e04a2-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e04a2-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e04a2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e04a2-137">Response</span></span>
<span data-ttu-id="e04a2-p108">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e04a2-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="e04a2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="e04a2-140">See also</span></span>

- [<span data-ttu-id="e04a2-141">Инструкции для выполнения проверки доступа</span><span class="sxs-lookup"><span data-stu-id="e04a2-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="e04a2-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e04a2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e04a2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e04a2-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="e04a2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e04a2-144">Response</span></span>
><span data-ttu-id="e04a2-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e04a2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
