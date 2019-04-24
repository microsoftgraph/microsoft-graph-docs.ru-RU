---
title: Список рецензентов Акцессревиев
description: В функции рецензирования Access в Azure AD извлеките проверяющих объект Акцессревиев.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459418"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="a9b50-103">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a9b50-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9b50-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлеките проверяющих объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a9b50-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9b50-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b50-105">Permissions</span></span>
<span data-ttu-id="a9b50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b50-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b50-108">Permission type</span></span>                        | <span data-ttu-id="a9b50-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9b50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9b50-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9b50-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9b50-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a9b50-111"></span></span>  <span data-ttu-id="a9b50-112">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать доступ.</span><span class="sxs-lookup"><span data-stu-id="a9b50-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="a9b50-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9b50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9b50-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b50-114">Not supported.</span></span> |
|<span data-ttu-id="a9b50-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9b50-115">Application</span></span>                            | <span data-ttu-id="a9b50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b50-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b50-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9b50-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="a9b50-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9b50-118">Request headers</span></span>
| <span data-ttu-id="a9b50-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a9b50-119">Name</span></span>         | <span data-ttu-id="a9b50-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a9b50-120">Type</span></span>        | <span data-ttu-id="a9b50-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b50-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a9b50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9b50-122">Authorization</span></span> | <span data-ttu-id="a9b50-123">string</span><span class="sxs-lookup"><span data-stu-id="a9b50-123">string</span></span> | <span data-ttu-id="a9b50-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9b50-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9b50-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9b50-126">Request body</span></span>
<span data-ttu-id="a9b50-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="a9b50-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a9b50-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b50-128">Response</span></span>
<span data-ttu-id="a9b50-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9b50-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b50-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a9b50-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9b50-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9b50-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="a9b50-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b50-132">Response</span></span>
><span data-ttu-id="a9b50-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9b50-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a9b50-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a9b50-135">See also</span></span>

| <span data-ttu-id="a9b50-136">Метод</span><span class="sxs-lookup"><span data-stu-id="a9b50-136">Method</span></span>           | <span data-ttu-id="a9b50-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a9b50-137">Return Type</span></span>    |<span data-ttu-id="a9b50-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b50-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9b50-139">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a9b50-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a9b50-140">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a9b50-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a9b50-141">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a9b50-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a9b50-142">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a9b50-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="a9b50-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="a9b50-143">None.</span></span>   |   <span data-ttu-id="a9b50-144">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="a9b50-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a9b50-145">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a9b50-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="a9b50-146">Нет.</span><span class="sxs-lookup"><span data-stu-id="a9b50-146">None.</span></span> |   <span data-ttu-id="a9b50-147">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="a9b50-147">Remove a reviewer from an accessReview.</span></span> |


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
