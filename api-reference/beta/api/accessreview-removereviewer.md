---
title: Удаление accessReview редактор
description: 'В Azure AD access дается обзор компонента "," Обновление существующего объекта accessReview для удаления пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 84bf3d973820067e0d4561e9647f688c025d957f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956691"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="d6431-105">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="d6431-105">Remove accessReview reviewer</span></span>

> <span data-ttu-id="d6431-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6431-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6431-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6431-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6431-108">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) для удаления пользователя в качестве читателя.</span><span class="sxs-lookup"><span data-stu-id="d6431-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="d6431-109">Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов.</span><span class="sxs-lookup"><span data-stu-id="d6431-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="d6431-110">Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов.</span><span class="sxs-lookup"><span data-stu-id="d6431-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d6431-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6431-111">Permissions</span></span>
<span data-ttu-id="d6431-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6431-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6431-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6431-114">Permission type</span></span>                        | <span data-ttu-id="d6431-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6431-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6431-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6431-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6431-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6431-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d6431-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6431-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6431-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6431-119">Not supported.</span></span> |
|<span data-ttu-id="d6431-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6431-120">Application</span></span>                            | <span data-ttu-id="d6431-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6431-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6431-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6431-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="d6431-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6431-123">Request headers</span></span>
| <span data-ttu-id="d6431-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d6431-124">Name</span></span>         | <span data-ttu-id="d6431-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d6431-125">Type</span></span>        | <span data-ttu-id="d6431-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d6431-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d6431-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6431-127">Authorization</span></span> | <span data-ttu-id="d6431-128">string</span><span class="sxs-lookup"><span data-stu-id="d6431-128">string</span></span> | <span data-ttu-id="d6431-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="d6431-129">Bearer \{token\}.</span></span> <span data-ttu-id="d6431-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6431-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6431-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6431-131">Request body</span></span>
<span data-ttu-id="d6431-132">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="d6431-132">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="d6431-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6431-133">Response</span></span>
<span data-ttu-id="d6431-134">Если успешно завершена, этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="d6431-134">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6431-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d6431-135">Example</span></span>

<span data-ttu-id="d6431-136">Это пример обновления одноразовый (не периодические) review доступа удаление ненужных редактор.</span><span class="sxs-lookup"><span data-stu-id="d6431-136">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="d6431-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6431-137">Request</span></span>
<span data-ttu-id="d6431-138">В URL-АДРЕСЕ запроса укажите идентификатор объекта accessReview, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6431-138">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="d6431-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6431-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
