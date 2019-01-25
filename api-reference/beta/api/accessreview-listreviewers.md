---
title: Список accessReview рецензентов
description: В Azure AD access дается обзор компонента, получения редакторов объект accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529280"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="4bd36-103">Список accessReview рецензентов</span><span class="sxs-lookup"><span data-stu-id="4bd36-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bd36-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечения рецензентов объект [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="4bd36-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bd36-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd36-105">Permissions</span></span>
<span data-ttu-id="4bd36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd36-108">Permission type</span></span>                        | <span data-ttu-id="4bd36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bd36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bd36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bd36-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bd36-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4bd36-111"></span></span>  <span data-ttu-id="4bd36-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="4bd36-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="4bd36-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bd36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd36-114">Not supported.</span></span> |
|<span data-ttu-id="4bd36-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bd36-115">Application</span></span>                            | <span data-ttu-id="4bd36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd36-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd36-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bd36-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="4bd36-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bd36-118">Request headers</span></span>
| <span data-ttu-id="4bd36-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4bd36-119">Name</span></span>         | <span data-ttu-id="4bd36-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4bd36-120">Type</span></span>        | <span data-ttu-id="4bd36-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4bd36-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4bd36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd36-122">Authorization</span></span> | <span data-ttu-id="4bd36-123">string</span><span class="sxs-lookup"><span data-stu-id="4bd36-123">string</span></span> | <span data-ttu-id="4bd36-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="4bd36-124">Bearer \{token\}.</span></span> <span data-ttu-id="4bd36-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bd36-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bd36-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bd36-126">Request body</span></span>
<span data-ttu-id="4bd36-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="4bd36-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4bd36-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bd36-128">Response</span></span>
<span data-ttu-id="4bd36-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [удостоверению пользователя](../resources/useridentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bd36-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd36-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4bd36-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bd36-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bd36-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="4bd36-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd36-132">Response</span></span>
><span data-ttu-id="4bd36-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bd36-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4bd36-135">См. также</span><span class="sxs-lookup"><span data-stu-id="4bd36-135">See also</span></span>

| <span data-ttu-id="4bd36-136">Метод</span><span class="sxs-lookup"><span data-stu-id="4bd36-136">Method</span></span>           | <span data-ttu-id="4bd36-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4bd36-137">Return Type</span></span>    |<span data-ttu-id="4bd36-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4bd36-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bd36-139">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="4bd36-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="4bd36-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="4bd36-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="4bd36-141">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="4bd36-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="4bd36-142">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="4bd36-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="4bd36-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="4bd36-143">None.</span></span>   |   <span data-ttu-id="4bd36-144">Добавьте проверяющий accessReview.</span><span class="sxs-lookup"><span data-stu-id="4bd36-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="4bd36-145">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="4bd36-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="4bd36-146">Нет.</span><span class="sxs-lookup"><span data-stu-id="4bd36-146">None.</span></span> |   <span data-ttu-id="4bd36-147">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="4bd36-147">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
