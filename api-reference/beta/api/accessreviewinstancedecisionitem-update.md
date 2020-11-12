---
title: Обновление АкцессревиевинстанцедеЦисионитем
description: Обновление существующего объекта АкцессревиевинстанцедеЦисионитем, для которого вызывающий пользователь является проверяющим.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c856cb899cb2379c9d0abf2cd459e289beea82c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000990"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="cd56d-103">Обновление АкцессревиевинстанцедеЦисионитем</span><span class="sxs-lookup"><span data-stu-id="cd56d-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="cd56d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd56d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd56d-105">Обновление решений Access, известных как [акцессревиевинстанцедеЦисионитемс](../resources/accessreviewinstancedecisionitem.md), для которых пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="cd56d-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="cd56d-106">Любые изменения, внесенные в **акцессревиевинстанцедеЦисионитем** , могут выполняться только вызываемыми пользователями, указанными в качестве проверяющего для родительского [акцессревиевинстанце](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="cd56d-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd56d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd56d-107">Permissions</span></span>
<span data-ttu-id="cd56d-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="cd56d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cd56d-109">Делегированные разрешения для личных учетных записей Майкрософт не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cd56d-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="cd56d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd56d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd56d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd56d-111">Permission type</span></span>                        | <span data-ttu-id="cd56d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd56d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd56d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd56d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd56d-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd56d-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="cd56d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd56d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd56d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd56d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd56d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd56d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="cd56d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd56d-118">Request headers</span></span>
| <span data-ttu-id="cd56d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cd56d-119">Name</span></span>         | <span data-ttu-id="cd56d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cd56d-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="cd56d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd56d-121">Authorization</span></span>|<span data-ttu-id="cd56d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd56d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cd56d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd56d-124">Content-type</span></span> | <span data-ttu-id="cd56d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd56d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd56d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd56d-127">Request body</span></span>
<span data-ttu-id="cd56d-128">В следующей таблице приведены свойства, принятые для обновления `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="cd56d-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="cd56d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd56d-129">Property</span></span>     | <span data-ttu-id="cd56d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd56d-130">Type</span></span>       | <span data-ttu-id="cd56d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd56d-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cd56d-132">решении</span><span class="sxs-lookup"><span data-stu-id="cd56d-132">decision</span></span>  | <span data-ttu-id="cd56d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cd56d-133">String</span></span> | <span data-ttu-id="cd56d-134">Решение о доступе к проверяемой сущности.</span><span class="sxs-lookup"><span data-stu-id="cd56d-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="cd56d-135">Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="cd56d-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="cd56d-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd56d-136">Required.</span></span>  |
|  <span data-ttu-id="cd56d-137">текста</span><span class="sxs-lookup"><span data-stu-id="cd56d-137">justification</span></span> | <span data-ttu-id="cd56d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cd56d-138">String</span></span> | <span data-ttu-id="cd56d-139">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="cd56d-139">Context of the review provided to admins.</span></span> <span data-ttu-id="cd56d-140">Является обязательным, если Жустификатионрекуиредонаппровал имеет значение true для Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="cd56d-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="cd56d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd56d-141">Response</span></span>
<span data-ttu-id="cd56d-142">В случае успешного выполнения этот метод возвращает `204, NoContent` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="cd56d-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="cd56d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd56d-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="cd56d-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="cd56d-144">Examples</span></span>

<span data-ttu-id="cd56d-145">Это пример утверждающего доступа для пользователя, представленного в `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="cd56d-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```

---

### <a name="response"></a><span data-ttu-id="cd56d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd56d-146">Response</span></span>
><span data-ttu-id="cd56d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd56d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
