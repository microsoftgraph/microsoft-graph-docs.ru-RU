---
title: Обновление legalHold
description: Обновление свойств объекта legalHold.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6f44bc276bdc3ae5f23ce3243127a38d4e7a6063
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446987"
---
# <a name="update-legalhold"></a><span data-ttu-id="7eeac-103">Обновление legalHold</span><span class="sxs-lookup"><span data-stu-id="7eeac-103">Update legalHold</span></span>

<span data-ttu-id="7eeac-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7eeac-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eeac-105">Обновление свойств объекта [legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="7eeac-105">Update the properties of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7eeac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7eeac-106">Permissions</span></span>

<span data-ttu-id="7eeac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eeac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eeac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7eeac-109">Permission type</span></span>|<span data-ttu-id="7eeac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7eeac-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eeac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7eeac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7eeac-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eeac-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7eeac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7eeac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eeac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eeac-114">Not supported.</span></span>|
|<span data-ttu-id="7eeac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7eeac-115">Application</span></span>|<span data-ttu-id="7eeac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eeac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eeac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7eeac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="request-headers"></a><span data-ttu-id="7eeac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7eeac-118">Request headers</span></span>

|<span data-ttu-id="7eeac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7eeac-119">Name</span></span>|<span data-ttu-id="7eeac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7eeac-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7eeac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7eeac-121">Authorization</span></span>|<span data-ttu-id="7eeac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eeac-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7eeac-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7eeac-124">Content-Type</span></span>|<span data-ttu-id="7eeac-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eeac-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eeac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7eeac-127">Request body</span></span>

<span data-ttu-id="7eeac-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7eeac-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7eeac-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7eeac-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7eeac-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7eeac-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="7eeac-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7eeac-131">Property</span></span>|<span data-ttu-id="7eeac-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7eeac-132">Type</span></span>|<span data-ttu-id="7eeac-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7eeac-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eeac-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="7eeac-134">contentQuery</span></span>|<span data-ttu-id="7eeac-135">String</span><span class="sxs-lookup"><span data-stu-id="7eeac-135">String</span></span>|<span data-ttu-id="7eeac-136">Запрос KQL, который указывает содержимое, которое должно быть в указанных расположениях.</span><span class="sxs-lookup"><span data-stu-id="7eeac-136">KQL query that specifies content to be held in the specified locations.</span></span> <span data-ttu-id="7eeac-137">Дополнительные сведения о KQL в eDiscovery см. в статье [Keyword queries and search conditions for Content Search and eDiscovery.](/microsoft-365/compliance/keyword-queries-and-search-conditions)</span><span class="sxs-lookup"><span data-stu-id="7eeac-137">For more information about KQL in eDiscovery, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span> <span data-ttu-id="7eeac-138">Чтобы удерживать все содержимое в указанных расположениях, оставьте **contentQuery пустым.**</span><span class="sxs-lookup"><span data-stu-id="7eeac-138">To hold all content in the specified locations, leave **contentQuery** blank.</span></span> |
|<span data-ttu-id="7eeac-139">description</span><span class="sxs-lookup"><span data-stu-id="7eeac-139">description</span></span>|<span data-ttu-id="7eeac-140">String</span><span class="sxs-lookup"><span data-stu-id="7eeac-140">String</span></span>| <span data-ttu-id="7eeac-141">Описание юридического удержания.</span><span class="sxs-lookup"><span data-stu-id="7eeac-141">The legal hold description.</span></span> |
|<span data-ttu-id="7eeac-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7eeac-142">displayName</span></span>|<span data-ttu-id="7eeac-143">String</span><span class="sxs-lookup"><span data-stu-id="7eeac-143">String</span></span>| <span data-ttu-id="7eeac-144">Отображение имени юридического удержания.</span><span class="sxs-lookup"><span data-stu-id="7eeac-144">The display name of the legal hold.</span></span> |
|<span data-ttu-id="7eeac-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7eeac-145">isEnabled</span></span>|<span data-ttu-id="7eeac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7eeac-146">Boolean</span></span>|<span data-ttu-id="7eeac-147">Указывает, включено ли удержание и активно ли оно поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eeac-147">Indicates whether the hold is enabled and actively holding content.</span></span> |

## <a name="response"></a><span data-ttu-id="7eeac-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="7eeac-148">Response</span></span>

<span data-ttu-id="7eeac-149">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7eeac-149">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7eeac-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="7eeac-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7eeac-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="7eeac-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_legalhold"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
Content-Type: application/json
Content-length: 295

{
  "description": "This is a description for a legalHold"
}
```

### <a name="response"></a><span data-ttu-id="7eeac-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eeac-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 204 No Content
```
