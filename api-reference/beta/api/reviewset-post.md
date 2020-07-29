---
title: Создание представления
description: Создание набора проверки обнаружения электронных данных.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c16ef3c9e325e3c144cdec532cc81e6e31623138
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510297"
---
# <a name="create-reviewset"></a><span data-ttu-id="e3389-103">Создание представления</span><span class="sxs-lookup"><span data-stu-id="e3389-103">Create reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3389-104">Создайте новый объект [Review](../resources/reviewset.md) .</span><span class="sxs-lookup"><span data-stu-id="e3389-104">Create a new [reviewSet](../resources/reviewset.md) object.</span></span> <span data-ttu-id="e3389-105">Текст запроса содержит отображаемое имя набора проверки, которое является единственным доступным для записи свойством.</span><span class="sxs-lookup"><span data-stu-id="e3389-105">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3389-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3389-106">Permissions</span></span>

<span data-ttu-id="e3389-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3389-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3389-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3389-109">Permission type</span></span>                        | <span data-ttu-id="e3389-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3389-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3389-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3389-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3389-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="e3389-112">User.Read</span></span> |
| <span data-ttu-id="e3389-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3389-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3389-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3389-114">Not supported.</span></span> |
| <span data-ttu-id="e3389-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3389-115">Application</span></span>                            | <span data-ttu-id="e3389-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3389-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3389-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3389-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3389-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3389-118">Request headers</span></span>

| <span data-ttu-id="e3389-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e3389-119">Name</span></span>       | <span data-ttu-id="e3389-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e3389-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e3389-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3389-121">Authorization</span></span> | <span data-ttu-id="e3389-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3389-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3389-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3389-124">Request body</span></span>

<span data-ttu-id="e3389-125">В тексте запроса добавьте представление объекта [Review](../resources/reviewset.md)в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3389-125">In the request body, supply JSON representation of the [reviewSet](../resources/reviewset.md).</span></span>  <span data-ttu-id="e3389-126">В следующей таблице перечислены обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="e3389-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="e3389-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3389-127">Property</span></span>     | <span data-ttu-id="e3389-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e3389-128">Type</span></span>        | <span data-ttu-id="e3389-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e3389-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3389-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e3389-130">displayName</span></span>  | <span data-ttu-id="e3389-131">string</span><span class="sxs-lookup"><span data-stu-id="e3389-131">string</span></span>      | <span data-ttu-id="e3389-132">Имя набора проверки.</span><span class="sxs-lookup"><span data-stu-id="e3389-132">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="e3389-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3389-133">Response</span></span>

<span data-ttu-id="e3389-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Review](../resources/reviewset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3389-134">If successful, this method returns a `201 Created` response code and a [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3389-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3389-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3389-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3389-136">Request</span></span>

<span data-ttu-id="e3389-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3389-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```

### <a name="response"></a><span data-ttu-id="e3389-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3389-138">Response</span></span>

<span data-ttu-id="e3389-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3389-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e3389-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3389-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
