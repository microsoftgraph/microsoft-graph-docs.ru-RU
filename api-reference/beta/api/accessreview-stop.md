---
title: Остановка accessReview
description: В Azure AD access дается обзор компонента, Остановка текущего активного accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  (Чтобы предотвратить запуск будущих экземпляры повторяющихся проверки доступа, обновите его, чтобы изменить его дату окончания).  После обеспечения доступа просмотрите останавливается, рецензентов больше не могут предоставить входные данные и решения проверки доступа можно применить.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 070f91faa411fcc6d98db419d1683a7fb6493859
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521840"
---
# <a name="stop-accessreview"></a><span data-ttu-id="6e8f6-106">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="6e8f6-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e8f6-107">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD Остановка текущего активного [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="6e8f6-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="6e8f6-108">Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="6e8f6-109">(Чтобы предотвратить повторяющихся проверки доступа запуск будущих экземпляры, [обновите его](accessreview-update.md) , чтобы изменить его дату окончания).</span><span class="sxs-lookup"><span data-stu-id="6e8f6-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="6e8f6-110">После обеспечения доступа просмотрите останавливается, рецензентов больше не могут предоставить входные данные и решения проверки доступа можно применить.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e8f6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8f6-111">Permissions</span></span>
<span data-ttu-id="6e8f6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e8f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e8f6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8f6-114">Permission type</span></span>                        | <span data-ttu-id="6e8f6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e8f6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e8f6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e8f6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e8f6-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e8f6-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="6e8f6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e8f6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e8f6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-119">Not supported.</span></span> |
|<span data-ttu-id="6e8f6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e8f6-120">Application</span></span>                            | <span data-ttu-id="6e8f6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e8f6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e8f6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="6e8f6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e8f6-123">Request headers</span></span>
| <span data-ttu-id="6e8f6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6e8f6-124">Name</span></span>         | <span data-ttu-id="6e8f6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6e8f6-125">Type</span></span>        | <span data-ttu-id="6e8f6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6e8f6-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6e8f6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e8f6-127">Authorization</span></span> | <span data-ttu-id="6e8f6-128">string</span><span class="sxs-lookup"><span data-stu-id="6e8f6-128">string</span></span> | <span data-ttu-id="6e8f6-129">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="6e8f6-129">Bearer \{token\}.</span></span> <span data-ttu-id="6e8f6-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e8f6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e8f6-131">Request body</span></span>
<span data-ttu-id="6e8f6-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6e8f6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e8f6-133">Response</span></span>
<span data-ttu-id="6e8f6-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e8f6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6e8f6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e8f6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e8f6-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="6e8f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e8f6-138">Response</span></span>
><span data-ttu-id="6e8f6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e8f6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
