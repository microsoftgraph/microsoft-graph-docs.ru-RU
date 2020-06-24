---
title: Обновление клаимсмаппингполици
description: Обновление свойств объекта Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f5434c73f7942a87babe21170bb2d82ca9f15c76
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846326"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="5d562-103">Обновление клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="5d562-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="5d562-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d562-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d562-105">Обновление свойств объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5d562-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d562-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d562-106">Permissions</span></span>

<span data-ttu-id="5d562-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5d562-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5d562-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d562-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d562-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d562-109">Permission type</span></span>                        | <span data-ttu-id="5d562-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d562-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d562-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d562-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d562-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d562-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5d562-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d562-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d562-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d562-114">Not supported.</span></span> |
| <span data-ttu-id="5d562-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d562-115">Application</span></span>                            | <span data-ttu-id="5d562-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d562-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d562-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d562-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d562-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d562-118">Request headers</span></span>

| <span data-ttu-id="5d562-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d562-119">Name</span></span>       | <span data-ttu-id="5d562-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d562-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5d562-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d562-121">Authorization</span></span> | <span data-ttu-id="5d562-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5d562-122">Bearer {token}</span></span> |
| <span data-ttu-id="5d562-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d562-123">Content-type</span></span> | <span data-ttu-id="5d562-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d562-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d562-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d562-125">Request body</span></span>

<span data-ttu-id="5d562-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5d562-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5d562-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5d562-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5d562-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5d562-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d562-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d562-129">Property</span></span>     | <span data-ttu-id="5d562-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5d562-130">Type</span></span>        | <span data-ttu-id="5d562-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5d562-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d562-132">RDLC</span><span class="sxs-lookup"><span data-stu-id="5d562-132">definition</span></span>|<span data-ttu-id="5d562-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d562-133">String collection</span></span>| <span data-ttu-id="5d562-134">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d562-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="5d562-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d562-135">Required.</span></span>|
|<span data-ttu-id="5d562-136">description</span><span class="sxs-lookup"><span data-stu-id="5d562-136">description</span></span>|<span data-ttu-id="5d562-137">String</span><span class="sxs-lookup"><span data-stu-id="5d562-137">String</span></span>| <span data-ttu-id="5d562-138">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d562-138">Description for this policy.</span></span>|
|<span data-ttu-id="5d562-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5d562-139">displayName</span></span>|<span data-ttu-id="5d562-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5d562-140">String</span></span>| <span data-ttu-id="5d562-141">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d562-141">Display name for this policy.</span></span> <span data-ttu-id="5d562-142">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="5d562-142">Required.</span></span>|
|<span data-ttu-id="5d562-143">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="5d562-143">isOrganizationDefault</span></span>|<span data-ttu-id="5d562-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d562-144">Boolean</span></span>|<span data-ttu-id="5d562-145">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="5d562-145">If set to true, activates this policy.</span></span> <span data-ttu-id="5d562-146">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d562-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="5d562-147">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="5d562-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="5d562-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d562-148">Response</span></span>

<span data-ttu-id="5d562-149">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="5d562-149">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="5d562-150">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="5d562-150">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d562-151">Пример</span><span class="sxs-lookup"><span data-stu-id="5d562-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d562-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d562-152">Request</span></span>

<span data-ttu-id="5d562-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d562-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d562-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d562-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="5d562-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d562-155">Response</span></span>

<span data-ttu-id="5d562-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d562-156">The following is an example of the response.</span></span>

> <span data-ttu-id="5d562-157">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5d562-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d562-158">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5d562-158">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update claimsmappingpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
