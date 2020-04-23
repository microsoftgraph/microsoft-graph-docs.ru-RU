---
title: Создание Усерфлов
description: Используйте этот API для создания нового Усерфлов.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 777adf601bf71676c505d1a9340f87b7575fc0c7
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218824"
---
# <a name="create-userflow"></a><span data-ttu-id="d7e87-103">Создание Усерфлов</span><span class="sxs-lookup"><span data-stu-id="d7e87-103">Create userFlow</span></span>

<span data-ttu-id="d7e87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e87-105">Создание нового объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="d7e87-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7e87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e87-106">Permissions</span></span>

<span data-ttu-id="d7e87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7e87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7e87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e87-109">Permission type</span></span>                        | <span data-ttu-id="d7e87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7e87-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d7e87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7e87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7e87-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d7e87-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="d7e87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7e87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7e87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7e87-114">Not supported.</span></span> |
| <span data-ttu-id="d7e87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7e87-115">Application</span></span>                            | <span data-ttu-id="d7e87-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d7e87-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7e87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7e87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="d7e87-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7e87-118">Request headers</span></span>

| <span data-ttu-id="d7e87-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d7e87-119">Name</span></span>          | <span data-ttu-id="d7e87-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e87-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d7e87-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7e87-121">Authorization</span></span> | <span data-ttu-id="d7e87-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7e87-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d7e87-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7e87-124">Content-type</span></span> | <span data-ttu-id="d7e87-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7e87-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7e87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7e87-127">Request body</span></span>

<span data-ttu-id="d7e87-128">В тексте запроса добавьте представление объекта [усерфлов](../resources/identityuserflow.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7e87-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7e87-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e87-129">Response</span></span>

<span data-ttu-id="d7e87-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7e87-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7e87-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d7e87-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7e87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7e87-132">Request</span></span>

<span data-ttu-id="d7e87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7e87-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7e87-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7e87-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7e87-135">C#</span><span class="sxs-lookup"><span data-stu-id="d7e87-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7e87-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7e87-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7e87-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7e87-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7e87-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e87-138">Response</span></span>

<span data-ttu-id="d7e87-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7e87-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d7e87-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7e87-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
