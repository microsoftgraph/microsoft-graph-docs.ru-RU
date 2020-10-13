---
title: Обновление Пермиссионгрантполици
description: Обновление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 0ccc47ff73b11fcbc0c465bb1dbe8979939511ac
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433667"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="0c23b-103">Обновление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="0c23b-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="0c23b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c23b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c23b-105">Обновление свойств объекта  [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c23b-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c23b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c23b-106">Permissions</span></span>

<span data-ttu-id="0c23b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c23b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c23b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c23b-109">Permission type</span></span>                        | <span data-ttu-id="0c23b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c23b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0c23b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c23b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c23b-112">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="0c23b-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="0c23b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c23b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c23b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c23b-114">Not supported.</span></span> |
| <span data-ttu-id="0c23b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c23b-115">Application</span></span>                            | <span data-ttu-id="0c23b-116">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="0c23b-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c23b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c23b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c23b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c23b-118">Request headers</span></span>

| <span data-ttu-id="0c23b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c23b-119">Name</span></span>           | <span data-ttu-id="0c23b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c23b-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0c23b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c23b-121">Authorization</span></span>  | <span data-ttu-id="0c23b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c23b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c23b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c23b-124">Request body</span></span>

<span data-ttu-id="0c23b-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0c23b-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0c23b-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0c23b-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0c23b-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0c23b-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c23b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c23b-128">Property</span></span>     | <span data-ttu-id="0c23b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0c23b-129">Type</span></span> |<span data-ttu-id="0c23b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0c23b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c23b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0c23b-131">displayName</span></span> | <span data-ttu-id="0c23b-132">String</span><span class="sxs-lookup"><span data-stu-id="0c23b-132">String</span></span> |<span data-ttu-id="0c23b-133">Отображаемое имя политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="0c23b-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="0c23b-134">description</span><span class="sxs-lookup"><span data-stu-id="0c23b-134">description</span></span> |<span data-ttu-id="0c23b-135">String</span><span class="sxs-lookup"><span data-stu-id="0c23b-135">String</span></span>| <span data-ttu-id="0c23b-136">Описание политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="0c23b-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="0c23b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c23b-137">Response</span></span>

<span data-ttu-id="0c23b-138">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c23b-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c23b-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c23b-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c23b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c23b-140">Request</span></span>

<span data-ttu-id="0c23b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c23b-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```

### <a name="response"></a><span data-ttu-id="0c23b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c23b-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
