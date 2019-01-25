---
title: Добавление accessReview редактор
description: 'В Azure AD access дается обзор компонента "," Обновление существующего объекта accessReview для добавления другого пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516366"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="4404c-105">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="4404c-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4404c-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) для добавления другого пользователя в качестве читателя.</span><span class="sxs-lookup"><span data-stu-id="4404c-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="4404c-107">Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов.</span><span class="sxs-lookup"><span data-stu-id="4404c-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="4404c-108">Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов.</span><span class="sxs-lookup"><span data-stu-id="4404c-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="4404c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4404c-109">Permissions</span></span>
<span data-ttu-id="4404c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4404c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4404c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4404c-112">Permission type</span></span>                        | <span data-ttu-id="4404c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4404c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4404c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4404c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4404c-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4404c-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4404c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4404c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4404c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4404c-117">Not supported.</span></span> |
|<span data-ttu-id="4404c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4404c-118">Application</span></span>                            | <span data-ttu-id="4404c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4404c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4404c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4404c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="4404c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4404c-121">Request headers</span></span>
| <span data-ttu-id="4404c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4404c-122">Name</span></span>         | <span data-ttu-id="4404c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4404c-123">Type</span></span>        | <span data-ttu-id="4404c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4404c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4404c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4404c-125">Authorization</span></span> | <span data-ttu-id="4404c-126">string</span><span class="sxs-lookup"><span data-stu-id="4404c-126">string</span></span> | <span data-ttu-id="4404c-127">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="4404c-127">Bearer \{token\}.</span></span> <span data-ttu-id="4404c-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4404c-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4404c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4404c-129">Request body</span></span>
<span data-ttu-id="4404c-130">В тексте запроса укажите JSON, представляющую идентификатор пользователя, который будет проверяющего.</span><span class="sxs-lookup"><span data-stu-id="4404c-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="4404c-131">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="4404c-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="4404c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4404c-132">Property</span></span>     | <span data-ttu-id="4404c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4404c-133">Type</span></span>        | <span data-ttu-id="4404c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4404c-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="4404c-135">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="4404c-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="4404c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4404c-136">Response</span></span>
<span data-ttu-id="4404c-137">Успешно завершена, этот метод возвращает `201, Created` код ответа.</span><span class="sxs-lookup"><span data-stu-id="4404c-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="4404c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4404c-138">Example</span></span>

<span data-ttu-id="4404c-139">Это пример обновления одноразовый (не периодические) review доступа с дополнительной редактор.</span><span class="sxs-lookup"><span data-stu-id="4404c-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="4404c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4404c-140">Request</span></span>
<span data-ttu-id="4404c-141">В тексте запроса укажите JSON, представляющую идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="4404c-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="4404c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4404c-142">Response</span></span>
><span data-ttu-id="4404c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4404c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
