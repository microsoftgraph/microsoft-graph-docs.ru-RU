---
title: Создание Активитибаседтимеаутполици
description: Создание нового Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 480ab012a6f58e378d0bf9085d994eddb51e539d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992937"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="11dea-103">Создание Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="11dea-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="11dea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11dea-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="11dea-105">Создание нового объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11dea-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11dea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11dea-106">Permissions</span></span>

<span data-ttu-id="11dea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11dea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11dea-109">Permission type</span></span>                        | <span data-ttu-id="11dea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11dea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11dea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11dea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11dea-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11dea-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="11dea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11dea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11dea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11dea-114">Not supported.</span></span> |
| <span data-ttu-id="11dea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11dea-115">Application</span></span>                            | <span data-ttu-id="11dea-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11dea-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="11dea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11dea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="11dea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11dea-118">Request headers</span></span>

| <span data-ttu-id="11dea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="11dea-119">Name</span></span>          | <span data-ttu-id="11dea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11dea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="11dea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11dea-121">Authorization</span></span> | <span data-ttu-id="11dea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11dea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11dea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11dea-124">Content-type</span></span> | <span data-ttu-id="11dea-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11dea-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11dea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11dea-127">Request body</span></span>

<span data-ttu-id="11dea-128">В тексте запроса добавьте представление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11dea-128">In the request body, supply a JSON representation of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11dea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="11dea-129">Response</span></span>

<span data-ttu-id="11dea-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11dea-130">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11dea-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="11dea-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11dea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="11dea-132">Request</span></span>

<span data-ttu-id="11dea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11dea-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11dea-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="11dea-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="11dea-135">C#</span><span class="sxs-lookup"><span data-stu-id="11dea-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11dea-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11dea-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11dea-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11dea-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11dea-138">Java</span><span class="sxs-lookup"><span data-stu-id="11dea-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11dea-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="11dea-139">Response</span></span>

<span data-ttu-id="11dea-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11dea-140">The following is an example of the response.</span></span>

> <span data-ttu-id="11dea-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11dea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

