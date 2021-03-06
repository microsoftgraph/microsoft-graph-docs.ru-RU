---
title: Обновление обзораSetQuery
description: Обновление свойств объекта reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 863a64bd0182d43c32756b6b214753a498d400df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515760"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="cdcbc-103">Обновление обзораSetQuery</span><span class="sxs-lookup"><span data-stu-id="cdcbc-103">Update reviewSetQuery</span></span>

<span data-ttu-id="cdcbc-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="cdcbc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdcbc-105">Обнови свойства обзора [eDiscoverySetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="cdcbc-105">Update the properties of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdcbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcbc-106">Permissions</span></span>

<span data-ttu-id="cdcbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdcbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcbc-109">Permission type</span></span>|<span data-ttu-id="cdcbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdcbc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdcbc-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdcbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdcbc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcbc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="cdcbc-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdcbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdcbc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-114">Not supported.</span></span>|
|<span data-ttu-id="cdcbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdcbc-115">Application</span></span>|<span data-ttu-id="cdcbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdcbc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cdcbc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdcbc-118">Request headers</span></span>

| <span data-ttu-id="cdcbc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cdcbc-119">Name</span></span>       | <span data-ttu-id="cdcbc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cdcbc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cdcbc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdcbc-121">Authorization</span></span> | <span data-ttu-id="cdcbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdcbc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdcbc-124">Request body</span></span>

<span data-ttu-id="cdcbc-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cdcbc-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cdcbc-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cdcbc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdcbc-128">Property</span></span>     | <span data-ttu-id="cdcbc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cdcbc-129">Type</span></span>        | <span data-ttu-id="cdcbc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cdcbc-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cdcbc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="cdcbc-131">displayName</span></span> | <span data-ttu-id="cdcbc-132">String</span><span class="sxs-lookup"><span data-stu-id="cdcbc-132">String</span></span> | <span data-ttu-id="cdcbc-133">Отображение имени для проверки набора запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-133">Display name for they review set query.</span></span> |
| <span data-ttu-id="cdcbc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcbc-134">query</span></span> | <span data-ttu-id="cdcbc-135">String</span><span class="sxs-lookup"><span data-stu-id="cdcbc-135">String</span></span> | <span data-ttu-id="cdcbc-136">Строка запроса в запросе KQL (Язык запросов ключевых слов).</span><span class="sxs-lookup"><span data-stu-id="cdcbc-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="cdcbc-137">Подробные сведения см. [в поле метаданных документа.](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="cdcbc-137">For details, see [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="cdcbc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdcbc-138">Response</span></span>

<span data-ttu-id="cdcbc-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdcbc-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdcbc-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdcbc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcbc-142">Request</span></span>

<span data-ttu-id="cdcbc-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```

### <a name="response"></a><span data-ttu-id="cdcbc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdcbc-144">Response</span></span>

<span data-ttu-id="cdcbc-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-145">The following is an example of the response.</span></span>

> <span data-ttu-id="cdcbc-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdcbc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
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