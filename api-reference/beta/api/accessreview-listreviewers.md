---
title: Список accessReview рецензентов
description: В Azure AD access дается обзор компонента, получения редакторов объект accessReview.
ms.openlocfilehash: 24c8b3dacbbe1a5868c9ba82141f37b006dc7a75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076324"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="10ef7-103">Список accessReview рецензентов</span><span class="sxs-lookup"><span data-stu-id="10ef7-103">List accessReview reviewers</span></span>

> <span data-ttu-id="10ef7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10ef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10ef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10ef7-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечения рецензентов объект [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="10ef7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10ef7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10ef7-107">Permissions</span></span>
<span data-ttu-id="10ef7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ef7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ef7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ef7-110">Permission type</span></span>                        | <span data-ttu-id="10ef7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ef7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10ef7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ef7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="10ef7-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="10ef7-113"></span></span>  <span data-ttu-id="10ef7-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="10ef7-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="10ef7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ef7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ef7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ef7-116">Not supported.</span></span> |
|<span data-ttu-id="10ef7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ef7-117">Application</span></span>                            | <span data-ttu-id="10ef7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ef7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ef7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ef7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="10ef7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ef7-120">Request headers</span></span>
| <span data-ttu-id="10ef7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="10ef7-121">Name</span></span>         | <span data-ttu-id="10ef7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="10ef7-122">Type</span></span>        | <span data-ttu-id="10ef7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="10ef7-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="10ef7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ef7-124">Authorization</span></span> | <span data-ttu-id="10ef7-125">string</span><span class="sxs-lookup"><span data-stu-id="10ef7-125">string</span></span> | <span data-ttu-id="10ef7-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="10ef7-126">Bearer \{token\}.</span></span> <span data-ttu-id="10ef7-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="10ef7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10ef7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ef7-128">Request body</span></span>
<span data-ttu-id="10ef7-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="10ef7-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="10ef7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="10ef7-130">Response</span></span>
<span data-ttu-id="10ef7-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [удостоверению пользователя](../resources/useridentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="10ef7-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ef7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10ef7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10ef7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ef7-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="10ef7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ef7-134">Response</span></span>
><span data-ttu-id="10ef7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10ef7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="10ef7-137">См. также</span><span class="sxs-lookup"><span data-stu-id="10ef7-137">See also</span></span>

| <span data-ttu-id="10ef7-138">Метод</span><span class="sxs-lookup"><span data-stu-id="10ef7-138">Method</span></span>           | <span data-ttu-id="10ef7-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="10ef7-139">Return Type</span></span>    |<span data-ttu-id="10ef7-140">Описание</span><span class="sxs-lookup"><span data-stu-id="10ef7-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10ef7-141">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="10ef7-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="10ef7-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="10ef7-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="10ef7-143">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="10ef7-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="10ef7-144">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="10ef7-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="10ef7-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="10ef7-145">None.</span></span>   |   <span data-ttu-id="10ef7-146">Добавьте проверяющий accessReview.</span><span class="sxs-lookup"><span data-stu-id="10ef7-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="10ef7-147">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="10ef7-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="10ef7-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="10ef7-148">None.</span></span> |   <span data-ttu-id="10ef7-149">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="10ef7-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
