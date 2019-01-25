---
title: Удаление accessReview редактор
description: 'В Azure AD access дается обзор компонента "," Обновление существующего объекта accessReview для удаления пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b6ea0fecb6b9179f40fa185aa770a743776eaa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523129"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="c1de8-105">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="c1de8-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1de8-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) для удаления пользователя в качестве читателя.</span><span class="sxs-lookup"><span data-stu-id="c1de8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="c1de8-107">Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов.</span><span class="sxs-lookup"><span data-stu-id="c1de8-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="c1de8-108">Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов.</span><span class="sxs-lookup"><span data-stu-id="c1de8-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c1de8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1de8-109">Permissions</span></span>
<span data-ttu-id="c1de8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1de8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1de8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1de8-112">Permission type</span></span>                        | <span data-ttu-id="c1de8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1de8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1de8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1de8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1de8-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1de8-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c1de8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1de8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1de8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1de8-117">Not supported.</span></span> |
|<span data-ttu-id="c1de8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1de8-118">Application</span></span>                            | <span data-ttu-id="c1de8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1de8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1de8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1de8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="c1de8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1de8-121">Request headers</span></span>
| <span data-ttu-id="c1de8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c1de8-122">Name</span></span>         | <span data-ttu-id="c1de8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c1de8-123">Type</span></span>        | <span data-ttu-id="c1de8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c1de8-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c1de8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1de8-125">Authorization</span></span> | <span data-ttu-id="c1de8-126">string</span><span class="sxs-lookup"><span data-stu-id="c1de8-126">string</span></span> | <span data-ttu-id="c1de8-127">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="c1de8-127">Bearer \{token\}.</span></span> <span data-ttu-id="c1de8-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1de8-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1de8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1de8-129">Request body</span></span>
<span data-ttu-id="c1de8-130">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="c1de8-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="c1de8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1de8-131">Response</span></span>
<span data-ttu-id="c1de8-132">Если успешно завершена, этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="c1de8-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="c1de8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c1de8-133">Example</span></span>

<span data-ttu-id="c1de8-134">Это пример обновления одноразовый (не периодические) review доступа удаление ненужных редактор.</span><span class="sxs-lookup"><span data-stu-id="c1de8-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="c1de8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1de8-135">Request</span></span>
<span data-ttu-id="c1de8-136">В URL-АДРЕСЕ запроса укажите идентификатор объекта accessReview, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1de8-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="c1de8-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1de8-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
