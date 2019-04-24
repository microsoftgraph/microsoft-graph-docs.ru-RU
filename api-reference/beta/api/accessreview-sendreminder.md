---
title: Сендреминдер Акцессревиев
description: 'В функции рецензирования Access Azure AD отправьте напоминание рецензентам, которые активны в настоящее время Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459426"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="073cd-104">Сендреминдер Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="073cd-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="073cd-105">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD отправьте напоминание рецензентам, которые активны в настоящее время [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="073cd-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="073cd-106">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="073cd-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="073cd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="073cd-107">Permissions</span></span>
<span data-ttu-id="073cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="073cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="073cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="073cd-110">Permission type</span></span>                        | <span data-ttu-id="073cd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="073cd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="073cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="073cd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="073cd-113">Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="073cd-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="073cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="073cd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="073cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="073cd-115">Not supported.</span></span> |
|<span data-ttu-id="073cd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="073cd-116">Application</span></span>                            | <span data-ttu-id="073cd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="073cd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="073cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="073cd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="073cd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="073cd-119">Request headers</span></span>
| <span data-ttu-id="073cd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="073cd-120">Name</span></span>         | <span data-ttu-id="073cd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="073cd-121">Type</span></span>        | <span data-ttu-id="073cd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="073cd-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="073cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="073cd-123">Authorization</span></span> | <span data-ttu-id="073cd-124">string</span><span class="sxs-lookup"><span data-stu-id="073cd-124">string</span></span> | <span data-ttu-id="073cd-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="073cd-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="073cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="073cd-127">Request body</span></span>
<span data-ttu-id="073cd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="073cd-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="073cd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="073cd-129">Response</span></span>
<span data-ttu-id="073cd-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="073cd-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073cd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="073cd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="073cd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="073cd-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="073cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="073cd-134">Response</span></span>
><span data-ttu-id="073cd-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="073cd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
