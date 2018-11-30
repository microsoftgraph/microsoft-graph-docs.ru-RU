---
title: Применение accessReview
description: 'В Azure AD доступ к функции проверки, применение решения завершенных accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  '
ms.openlocfilehash: 2a5675eee989e21fcc275ddf859738af46742610
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076330"
---
# <a name="apply-accessreview"></a><span data-ttu-id="5f06c-104">Применение accessReview</span><span class="sxs-lookup"><span data-stu-id="5f06c-104">Apply accessReview</span></span>

> <span data-ttu-id="5f06c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f06c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f06c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f06c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f06c-107">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD применение решения завершенных [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="5f06c-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="5f06c-108">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5f06c-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="5f06c-109">После завершения проверки доступа, либо так, как связаться с вами дату окончания или администратор остановлена вручную и автоматически назначаемой не был настроен на проверку, можно вызвать применить, чтобы применить изменения.</span><span class="sxs-lookup"><span data-stu-id="5f06c-109">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="5f06c-110">Пока не происходит применить о решениях для удаления права доступа не отображаются на ресурсов источника, пользователей, например сохранять их членства в группе.</span><span class="sxs-lookup"><span data-stu-id="5f06c-110">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="5f06c-111">Путем вызова применения, результат проверки реализована путем обновления группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="5f06c-111">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="5f06c-112">Если нет доступа пользователя в разделе review, когда администратор вызывает этот интерфейс API, Azure AD удалит их назначения членства или приложения.</span><span class="sxs-lookup"><span data-stu-id="5f06c-112">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="5f06c-113">После проверки доступа по завершении работы и автоматически назначаемой был настроен, то состояние проверки будет заменен завершено промежуточного состояния и наконец изменится на состояние применения.</span><span class="sxs-lookup"><span data-stu-id="5f06c-113">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="5f06c-114">При любой, удаляемого из ресурса групповой членства или приложение назначения всего за несколько минут должно привести для просмотра запрещенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="5f06c-114">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="5f06c-115">Настроенные автоматическое применение проверки или выбор применить не влияет на группы, которая исходит в локальном каталоге или динамические группы.</span><span class="sxs-lookup"><span data-stu-id="5f06c-115">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="5f06c-116">Если вы хотите изменить группу, которая исходит локальной, загрузите результаты и применить эти изменения к представление группы в этой папке.</span><span class="sxs-lookup"><span data-stu-id="5f06c-116">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="5f06c-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f06c-117">Permissions</span></span>
<span data-ttu-id="5f06c-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f06c-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f06c-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f06c-120">Permission type</span></span>                        | <span data-ttu-id="5f06c-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f06c-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f06c-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f06c-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f06c-123">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f06c-123">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="5f06c-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f06c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f06c-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f06c-125">Not supported.</span></span> |
|<span data-ttu-id="5f06c-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f06c-126">Application</span></span>                            | <span data-ttu-id="5f06c-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f06c-127">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f06c-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f06c-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="5f06c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f06c-129">Request headers</span></span>
| <span data-ttu-id="5f06c-130">Имя</span><span class="sxs-lookup"><span data-stu-id="5f06c-130">Name</span></span>         | <span data-ttu-id="5f06c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5f06c-131">Type</span></span>        | <span data-ttu-id="5f06c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5f06c-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5f06c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f06c-133">Authorization</span></span> | <span data-ttu-id="5f06c-134">string</span><span class="sxs-lookup"><span data-stu-id="5f06c-134">string</span></span> | <span data-ttu-id="5f06c-135">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="5f06c-135">Bearer \{token\}.</span></span> <span data-ttu-id="5f06c-136">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5f06c-136">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f06c-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f06c-137">Request body</span></span>
<span data-ttu-id="5f06c-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f06c-138">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5f06c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f06c-139">Response</span></span>
<span data-ttu-id="5f06c-p109">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5f06c-p109">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f06c-142">См. также</span><span class="sxs-lookup"><span data-stu-id="5f06c-142">See also</span></span>

- [<span data-ttu-id="5f06c-143">Инструкции для выполнения проверки доступа</span><span class="sxs-lookup"><span data-stu-id="5f06c-143">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="5f06c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5f06c-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f06c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f06c-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="5f06c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f06c-146">Response</span></span>
><span data-ttu-id="5f06c-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f06c-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
