---
title: Создание Активитибаседтимеаутполици
description: Создание нового Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da819249d9ae4ea59eee913af9bed1f6fef4f879
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234449"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="68c6b-103">Создание Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="68c6b-103">Create activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68c6b-104">Создание нового объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="68c6b-104">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="68c6b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68c6b-105">Permissions</span></span>

<span data-ttu-id="68c6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68c6b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c6b-108">Permission type</span></span>                        | <span data-ttu-id="68c6b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c6b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68c6b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c6b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="68c6b-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="68c6b-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="68c6b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68c6b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c6b-113">Not supported.</span></span> |
| <span data-ttu-id="68c6b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68c6b-114">Application</span></span>                            | <span data-ttu-id="68c6b-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="68c6b-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="68c6b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c6b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="68c6b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68c6b-117">Request headers</span></span>

| <span data-ttu-id="68c6b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="68c6b-118">Name</span></span>          | <span data-ttu-id="68c6b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="68c6b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68c6b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68c6b-120">Authorization</span></span> | <span data-ttu-id="68c6b-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="68c6b-121">Bearer {token}</span></span> |
| <span data-ttu-id="68c6b-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68c6b-122">Content-type</span></span> | <span data-ttu-id="68c6b-123">application/json</span><span class="sxs-lookup"><span data-stu-id="68c6b-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="68c6b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68c6b-124">Request body</span></span>

<span data-ttu-id="68c6b-125">В тексте запроса добавьте представление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68c6b-125">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68c6b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c6b-126">Response</span></span>

<span data-ttu-id="68c6b-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68c6b-127">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68c6b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="68c6b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68c6b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c6b-129">Request</span></span>

<span data-ttu-id="68c6b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c6b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="68c6b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c6b-131">Response</span></span>

<span data-ttu-id="68c6b-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68c6b-132">The following is an example of the response.</span></span>

> <span data-ttu-id="68c6b-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c6b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->