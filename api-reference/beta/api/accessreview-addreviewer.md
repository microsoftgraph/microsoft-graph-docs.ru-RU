---
title: Добавление accessReview редактор
description: 'В Azure AD access дается обзор компонента "," Обновление существующего объекта accessReview для добавления другого пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. '
ms.openlocfilehash: ac7722d1bea30659db6f6defe26c0a08ecd67caf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077313"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="b2778-105">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="b2778-105">Add accessReview reviewer</span></span>

> <span data-ttu-id="b2778-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2778-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2778-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2778-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2778-108">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) для добавления другого пользователя в качестве читателя.</span><span class="sxs-lookup"><span data-stu-id="b2778-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="b2778-109">Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов.</span><span class="sxs-lookup"><span data-stu-id="b2778-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="b2778-110">Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов.</span><span class="sxs-lookup"><span data-stu-id="b2778-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="b2778-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2778-111">Permissions</span></span>
<span data-ttu-id="b2778-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2778-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2778-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2778-114">Permission type</span></span>                        | <span data-ttu-id="b2778-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2778-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2778-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2778-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2778-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2778-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b2778-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2778-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2778-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2778-119">Not supported.</span></span> |
|<span data-ttu-id="b2778-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2778-120">Application</span></span>                            | <span data-ttu-id="b2778-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2778-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2778-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2778-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="b2778-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2778-123">Request headers</span></span>
| <span data-ttu-id="b2778-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b2778-124">Name</span></span>         | <span data-ttu-id="b2778-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b2778-125">Type</span></span>        | <span data-ttu-id="b2778-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b2778-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b2778-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2778-127">Authorization</span></span> | <span data-ttu-id="b2778-128">string</span><span class="sxs-lookup"><span data-stu-id="b2778-128">string</span></span> | <span data-ttu-id="b2778-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="b2778-129">Bearer \{token\}.</span></span> <span data-ttu-id="b2778-130">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="b2778-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2778-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2778-131">Request body</span></span>
<span data-ttu-id="b2778-132">В тексте запроса укажите JSON, представляющую идентификатор пользователя, который будет проверяющего.</span><span class="sxs-lookup"><span data-stu-id="b2778-132">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="b2778-133">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="b2778-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="b2778-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2778-134">Property</span></span>     | <span data-ttu-id="b2778-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b2778-135">Type</span></span>        | <span data-ttu-id="b2778-136">Description</span><span class="sxs-lookup"><span data-stu-id="b2778-136">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="b2778-137">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2778-137">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="b2778-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2778-138">Response</span></span>
<span data-ttu-id="b2778-139">Успешно завершена, этот метод возвращает `201, Created` код ответа.</span><span class="sxs-lookup"><span data-stu-id="b2778-139">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="b2778-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b2778-140">Example</span></span>

<span data-ttu-id="b2778-141">Это пример обновления одноразовый (не периодические) review доступа с дополнительной редактор.</span><span class="sxs-lookup"><span data-stu-id="b2778-141">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="b2778-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2778-142">Request</span></span>
<span data-ttu-id="b2778-143">В тексте запроса укажите JSON, представляющую идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2778-143">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b2778-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2778-144">Response</span></span>
><span data-ttu-id="b2778-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2778-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
