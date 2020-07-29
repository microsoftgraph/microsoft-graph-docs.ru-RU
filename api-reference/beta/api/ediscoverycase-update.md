---
title: Обновление едисковерикасе
description: Обновление свойств объекта Едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f0df9131046d8c031a492502c64c2272e4761bf0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510201"
---
# <a name="update-ediscoverycase"></a><span data-ttu-id="90de9-103">Обновление Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="90de9-103">Update ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90de9-104">Обновление свойств объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="90de9-104">Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90de9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90de9-105">Permissions</span></span>

<span data-ttu-id="90de9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90de9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90de9-108">Permission type</span></span>                        | <span data-ttu-id="90de9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90de9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90de9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90de9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="90de9-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="90de9-111">User.Read</span></span>      |
| <span data-ttu-id="90de9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90de9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90de9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90de9-113">Not supported.</span></span> |
| <span data-ttu-id="90de9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90de9-114">Application</span></span>                            | <span data-ttu-id="90de9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90de9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90de9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90de9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90de9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90de9-117">Request headers</span></span>

| <span data-ttu-id="90de9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="90de9-118">Name</span></span>       | <span data-ttu-id="90de9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="90de9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="90de9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90de9-120">Authorization</span></span> | <span data-ttu-id="90de9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90de9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90de9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90de9-123">Request body</span></span>

<span data-ttu-id="90de9-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="90de9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="90de9-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="90de9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="90de9-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="90de9-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="90de9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="90de9-127">Property</span></span>     | <span data-ttu-id="90de9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="90de9-128">Type</span></span>        | <span data-ttu-id="90de9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="90de9-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90de9-130">description</span><span class="sxs-lookup"><span data-stu-id="90de9-130">description</span></span>|<span data-ttu-id="90de9-131">String</span><span class="sxs-lookup"><span data-stu-id="90de9-131">String</span></span>| <span data-ttu-id="90de9-132">Описание варианта.</span><span class="sxs-lookup"><span data-stu-id="90de9-132">The case description.</span></span> |
|<span data-ttu-id="90de9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="90de9-133">displayName</span></span>|<span data-ttu-id="90de9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="90de9-134">String</span></span>| <span data-ttu-id="90de9-135">Имя дела.</span><span class="sxs-lookup"><span data-stu-id="90de9-135">The case name.</span></span> |
|<span data-ttu-id="90de9-136">externalId</span><span class="sxs-lookup"><span data-stu-id="90de9-136">externalId</span></span>|<span data-ttu-id="90de9-137">String</span><span class="sxs-lookup"><span data-stu-id="90de9-137">String</span></span>| <span data-ttu-id="90de9-138">Номер внешнего обращения для ссылки на клиента.</span><span class="sxs-lookup"><span data-stu-id="90de9-138">The external case number for customer reference.</span></span> |

## <a name="response"></a><span data-ttu-id="90de9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="90de9-139">Response</span></span>

<span data-ttu-id="90de9-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90de9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90de9-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="90de9-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90de9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="90de9-143">Request</span></span>

<span data-ttu-id="90de9-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90de9-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```

### <a name="response"></a><span data-ttu-id="90de9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="90de9-145">Response</span></span>

<span data-ttu-id="90de9-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90de9-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ediscoverycase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
