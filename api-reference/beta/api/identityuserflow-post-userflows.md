---
title: Создание Усерфлов
description: Используйте этот API для создания нового Усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cd660e4be738469351e3d1369d557774895ac58
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938572"
---
# <a name="create-userflow"></a><span data-ttu-id="11a97-103">Создание Усерфлов</span><span class="sxs-lookup"><span data-stu-id="11a97-103">Create userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a97-104">Создание нового объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="11a97-104">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11a97-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11a97-105">Permissions</span></span>

<span data-ttu-id="11a97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11a97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11a97-108">Permission type</span></span>                        | <span data-ttu-id="11a97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11a97-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11a97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11a97-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11a97-111">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="11a97-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="11a97-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11a97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11a97-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11a97-113">Not supported.</span></span> |
| <span data-ttu-id="11a97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11a97-114">Application</span></span>                            | <span data-ttu-id="11a97-115">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="11a97-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11a97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11a97-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="11a97-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11a97-117">Request headers</span></span>

| <span data-ttu-id="11a97-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11a97-118">Name</span></span>          | <span data-ttu-id="11a97-119">Описание</span><span class="sxs-lookup"><span data-stu-id="11a97-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="11a97-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11a97-120">Authorization</span></span> | <span data-ttu-id="11a97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11a97-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="11a97-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11a97-123">Content-type</span></span> | <span data-ttu-id="11a97-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11a97-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11a97-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11a97-126">Request body</span></span>

<span data-ttu-id="11a97-127">В тексте запроса добавьте представление объекта [усерфлов](../resources/identityuserflow.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11a97-127">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11a97-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="11a97-128">Response</span></span>

<span data-ttu-id="11a97-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11a97-129">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11a97-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="11a97-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11a97-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="11a97-131">Request</span></span>

<span data-ttu-id="11a97-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11a97-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11a97-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="11a97-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11a97-134">C#</span><span class="sxs-lookup"><span data-stu-id="11a97-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11a97-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11a97-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11a97-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11a97-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11a97-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="11a97-137">Response</span></span>

<span data-ttu-id="11a97-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11a97-138">The following is an example of the response.</span></span>

> <span data-ttu-id="11a97-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11a97-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_identityuserflow_from_identitycontainer/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
