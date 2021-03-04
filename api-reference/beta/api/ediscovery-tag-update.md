---
title: Тег обновления
description: Обновление свойств объекта тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1cfc1fc24ea6e850daac08f9c741b2943b1e34d4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446828"
---
# <a name="update-tag"></a><span data-ttu-id="21b41-103">Тег обновления</span><span class="sxs-lookup"><span data-stu-id="21b41-103">Update tag</span></span>

<span data-ttu-id="21b41-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="21b41-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21b41-105">Обновление свойств объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="21b41-105">Update the properties of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21b41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21b41-106">Permissions</span></span>

<span data-ttu-id="21b41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21b41-109">Permission type</span></span>|<span data-ttu-id="21b41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21b41-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21b41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21b41-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21b41-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b41-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="21b41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21b41-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b41-114">Not supported.</span></span>|
|<span data-ttu-id="21b41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21b41-115">Application</span></span>|<span data-ttu-id="21b41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b41-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21b41-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="request-headers"></a><span data-ttu-id="21b41-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21b41-118">Request headers</span></span>

|<span data-ttu-id="21b41-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21b41-119">Name</span></span>|<span data-ttu-id="21b41-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21b41-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="21b41-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21b41-121">Authorization</span></span>|<span data-ttu-id="21b41-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21b41-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="21b41-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21b41-124">Content-Type</span></span>|<span data-ttu-id="21b41-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21b41-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21b41-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21b41-127">Request body</span></span>

<span data-ttu-id="21b41-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="21b41-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="21b41-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="21b41-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="21b41-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="21b41-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="21b41-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="21b41-131">Property</span></span>|<span data-ttu-id="21b41-132">Тип</span><span class="sxs-lookup"><span data-stu-id="21b41-132">Type</span></span>|<span data-ttu-id="21b41-133">Описание</span><span class="sxs-lookup"><span data-stu-id="21b41-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21b41-134">description</span><span class="sxs-lookup"><span data-stu-id="21b41-134">description</span></span>|<span data-ttu-id="21b41-135">String</span><span class="sxs-lookup"><span data-stu-id="21b41-135">String</span></span>|<span data-ttu-id="21b41-136">Описание тега.</span><span class="sxs-lookup"><span data-stu-id="21b41-136">The description for the tag.</span></span>|
|<span data-ttu-id="21b41-137">displayName</span><span class="sxs-lookup"><span data-stu-id="21b41-137">displayName</span></span>|<span data-ttu-id="21b41-138">String</span><span class="sxs-lookup"><span data-stu-id="21b41-138">String</span></span>|<span data-ttu-id="21b41-139">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="21b41-139">Display name of the tag.</span></span>|

## <a name="response"></a><span data-ttu-id="21b41-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="21b41-140">Response</span></span>

<span data-ttu-id="21b41-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21b41-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="21b41-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="21b41-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21b41-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="21b41-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tag"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
Content-Type: application/json
Content-length: 210

{
  "description":"This is an updated description."
}
```

### <a name="response"></a><span data-ttu-id="21b41-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="21b41-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
