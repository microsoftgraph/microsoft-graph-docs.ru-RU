---
title: SendReminder accessReview
description: 'Доступ к функции проверки в Azure AD, отправьте напоминание рецензентов текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518550"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="62cc2-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="62cc2-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62cc2-105">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD отправьте напоминание рецензентов текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="62cc2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="62cc2-106">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="62cc2-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="62cc2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62cc2-107">Permissions</span></span>
<span data-ttu-id="62cc2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62cc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62cc2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62cc2-110">Permission type</span></span>                        | <span data-ttu-id="62cc2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62cc2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="62cc2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62cc2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="62cc2-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cc2-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="62cc2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62cc2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62cc2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62cc2-115">Not supported.</span></span> |
|<span data-ttu-id="62cc2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62cc2-116">Application</span></span>                            | <span data-ttu-id="62cc2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62cc2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62cc2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62cc2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="62cc2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62cc2-119">Request headers</span></span>
| <span data-ttu-id="62cc2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="62cc2-120">Name</span></span>         | <span data-ttu-id="62cc2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="62cc2-121">Type</span></span>        | <span data-ttu-id="62cc2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="62cc2-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="62cc2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62cc2-123">Authorization</span></span> | <span data-ttu-id="62cc2-124">string</span><span class="sxs-lookup"><span data-stu-id="62cc2-124">string</span></span> | <span data-ttu-id="62cc2-125">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="62cc2-125">Bearer \{token\}.</span></span> <span data-ttu-id="62cc2-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62cc2-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62cc2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62cc2-127">Request body</span></span>
<span data-ttu-id="62cc2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62cc2-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="62cc2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="62cc2-129">Response</span></span>
<span data-ttu-id="62cc2-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="62cc2-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62cc2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="62cc2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62cc2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="62cc2-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="62cc2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="62cc2-134">Response</span></span>
><span data-ttu-id="62cc2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62cc2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
