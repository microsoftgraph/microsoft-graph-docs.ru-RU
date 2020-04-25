---
title: Создание Токенлифетимеполици
description: Создание нового Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db33f9a5e02e2e5b7763f412be3dd7e49669a003
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806082"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="db0ab-103">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="db0ab-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="db0ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db0ab-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="db0ab-105">Создание нового объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="db0ab-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db0ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db0ab-106">Permissions</span></span>

<span data-ttu-id="db0ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db0ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db0ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db0ab-109">Permission type</span></span>                        | <span data-ttu-id="db0ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db0ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db0ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db0ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db0ab-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0ab-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="db0ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db0ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db0ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db0ab-114">Not supported.</span></span> |
| <span data-ttu-id="db0ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db0ab-115">Application</span></span>                            | <span data-ttu-id="db0ab-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0ab-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="db0ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db0ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="db0ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db0ab-118">Request headers</span></span>

| <span data-ttu-id="db0ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="db0ab-119">Name</span></span>          | <span data-ttu-id="db0ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="db0ab-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db0ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db0ab-121">Authorization</span></span> | <span data-ttu-id="db0ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db0ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db0ab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db0ab-124">Content-type</span></span> | <span data-ttu-id="db0ab-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db0ab-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db0ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db0ab-127">Request body</span></span>

<span data-ttu-id="db0ab-128">В тексте запроса добавьте представление объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db0ab-128">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db0ab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="db0ab-129">Response</span></span>

<span data-ttu-id="db0ab-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db0ab-130">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db0ab-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="db0ab-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db0ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db0ab-132">Request</span></span>

<span data-ttu-id="db0ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db0ab-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db0ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db0ab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="db0ab-135">C#</span><span class="sxs-lookup"><span data-stu-id="db0ab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db0ab-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db0ab-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db0ab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db0ab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db0ab-138">Java</span><span class="sxs-lookup"><span data-stu-id="db0ab-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db0ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="db0ab-139">Response</span></span>

<span data-ttu-id="db0ab-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db0ab-140">The following is an example of the response.</span></span>

> <span data-ttu-id="db0ab-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db0ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
