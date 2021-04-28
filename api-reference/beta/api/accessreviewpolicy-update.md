---
title: Обновление accessReviewPolicy
description: Обновление свойств объекта accessReviewPolicy.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3a4ef900a4dfc88b28dfd3d11f96804655160823
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067621"
---
# <a name="update-accessreviewpolicy"></a><span data-ttu-id="b38fc-103">Обновление accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="b38fc-103">Update accessReviewPolicy</span></span>
<span data-ttu-id="b38fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b38fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b38fc-105">Обновление свойств объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b38fc-105">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b38fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b38fc-106">Permissions</span></span>
<span data-ttu-id="b38fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b38fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b38fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b38fc-109">Permission type</span></span>|<span data-ttu-id="b38fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b38fc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b38fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b38fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b38fc-112">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="b38fc-112">Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="b38fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b38fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b38fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b38fc-114">Not supported.</span></span>|
|<span data-ttu-id="b38fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b38fc-115">Application</span></span>|<span data-ttu-id="b38fc-116">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="b38fc-116">Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="b38fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b38fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/accessReviewPolicy
PATCH /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="b38fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b38fc-118">Request headers</span></span>
|<span data-ttu-id="b38fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b38fc-119">Name</span></span>|<span data-ttu-id="b38fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b38fc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b38fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b38fc-121">Authorization</span></span>|<span data-ttu-id="b38fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b38fc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b38fc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b38fc-124">Content-Type</span></span>|<span data-ttu-id="b38fc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b38fc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b38fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b38fc-127">Request body</span></span>
<span data-ttu-id="b38fc-128">В теле запроса поставляем представление JSON объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b38fc-128">In the request body, supply a JSON representation of the [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

<span data-ttu-id="b38fc-129">В следующей таблице показаны свойства, необходимые при обновлении [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b38fc-129">The following table shows the properties that are required when you update the [accessReviewPolicy](../resources/accessreviewpolicy.md).</span></span>

|<span data-ttu-id="b38fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b38fc-130">Property</span></span>|<span data-ttu-id="b38fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b38fc-131">Type</span></span>|<span data-ttu-id="b38fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b38fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b38fc-133">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="b38fc-133">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="b38fc-134">Логический</span><span class="sxs-lookup"><span data-stu-id="b38fc-134">Boolean</span></span>|<span data-ttu-id="b38fc-135">Если `true` владельцы групп могут создавать и управлять отзывами доступа в группах, которые им принадлежат.</span><span class="sxs-lookup"><span data-stu-id="b38fc-135">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|



## <a name="response"></a><span data-ttu-id="b38fc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b38fc-136">Response</span></span>

<span data-ttu-id="b38fc-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b38fc-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b38fc-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="b38fc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b38fc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b38fc-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/accessReviewPolicy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="b38fc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b38fc-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="request"></a><span data-ttu-id="b38fc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b38fc-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy_2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="b38fc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b38fc-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
