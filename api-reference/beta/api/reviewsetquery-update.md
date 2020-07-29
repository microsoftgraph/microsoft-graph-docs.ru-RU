---
title: Обновление Ревиевсеткуери
description: Обновление свойств объекта Ревиевсеткуери.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9ba2a3f51bee694001fde5f7f62f0f452aa0bcff
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510270"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="1e074-103">Обновление Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="1e074-103">Update reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e074-104">Обновление свойств [Ревиевсеткуери](../resources/reviewsetquery.md)обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="1e074-104">Update the properties of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e074-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e074-105">Permissions</span></span>

<span data-ttu-id="1e074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e074-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e074-108">Permission type</span></span>                        | <span data-ttu-id="1e074-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e074-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1e074-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e074-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e074-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="1e074-111">User.Read</span></span> |
| <span data-ttu-id="1e074-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e074-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e074-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e074-113">Not supported.</span></span> |
| <span data-ttu-id="1e074-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e074-114">Application</span></span>                            | <span data-ttu-id="1e074-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e074-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e074-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e074-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e074-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e074-117">Request headers</span></span>

| <span data-ttu-id="1e074-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1e074-118">Name</span></span>       | <span data-ttu-id="1e074-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1e074-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e074-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e074-120">Authorization</span></span> | <span data-ttu-id="1e074-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e074-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e074-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e074-123">Request body</span></span>

<span data-ttu-id="1e074-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1e074-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1e074-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1e074-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1e074-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1e074-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e074-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e074-127">Property</span></span>     | <span data-ttu-id="1e074-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1e074-128">Type</span></span>        | <span data-ttu-id="1e074-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1e074-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1e074-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1e074-130">displayName</span></span> | <span data-ttu-id="1e074-131">Строка</span><span class="sxs-lookup"><span data-stu-id="1e074-131">String</span></span> | <span data-ttu-id="1e074-132">Отображаемое имя Просмотр запроса Set.</span><span class="sxs-lookup"><span data-stu-id="1e074-132">Display name for they review set query.</span></span> |
| <span data-ttu-id="1e074-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e074-133">query</span></span> | <span data-ttu-id="1e074-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e074-134">String</span></span> | <span data-ttu-id="1e074-135">Строка запроса в запросе KQL (ключевое слово языка запросов).</span><span class="sxs-lookup"><span data-stu-id="1e074-135">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="1e074-136">Подробнее: [поля метаданных документа](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="1e074-136">For details, see [Document metadata fields](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="1e074-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e074-137">Response</span></span>

<span data-ttu-id="1e074-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1e074-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e074-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="1e074-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e074-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e074-141">Request</span></span>

<span data-ttu-id="1e074-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e074-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```

### <a name="response"></a><span data-ttu-id="1e074-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e074-143">Response</span></span>

<span data-ttu-id="1e074-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1e074-144">The following is an example of the response.</span></span>

> <span data-ttu-id="1e074-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e074-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewsetquery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
