---
title: Создание userFlow
description: Используйте этот API для создания нового пользовательского процесса.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36ccf24fb65a0098ebccb8774c36af804aece41f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176537"
---
# <a name="create-userflow"></a><span data-ttu-id="0393b-103">Создание userFlow</span><span class="sxs-lookup"><span data-stu-id="0393b-103">Create userFlow</span></span>

<span data-ttu-id="0393b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0393b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0393b-105">Создание объекта [userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="0393b-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0393b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0393b-106">Permissions</span></span>

<span data-ttu-id="0393b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0393b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0393b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0393b-109">Permission type</span></span>                        | <span data-ttu-id="0393b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0393b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0393b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0393b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0393b-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0393b-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="0393b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0393b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0393b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0393b-114">Not supported.</span></span> |
| <span data-ttu-id="0393b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0393b-115">Application</span></span>                            | <span data-ttu-id="0393b-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0393b-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0393b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0393b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="0393b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0393b-118">Request headers</span></span>

| <span data-ttu-id="0393b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0393b-119">Name</span></span>          | <span data-ttu-id="0393b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0393b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0393b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0393b-121">Authorization</span></span> | <span data-ttu-id="0393b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0393b-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="0393b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0393b-124">Content-type</span></span> | <span data-ttu-id="0393b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0393b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0393b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0393b-127">Request body</span></span>

<span data-ttu-id="0393b-128">В теле запроса укажу представление объекта [userFlow](../resources/identityuserflow.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="0393b-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0393b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0393b-129">Response</span></span>

<span data-ttu-id="0393b-130">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект userFlow](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0393b-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0393b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0393b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0393b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0393b-132">Request</span></span>

<span data-ttu-id="0393b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0393b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0393b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0393b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "id": "Pol1",
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="0393b-135">C#</span><span class="sxs-lookup"><span data-stu-id="0393b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0393b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0393b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0393b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0393b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0393b-138">Java</span><span class="sxs-lookup"><span data-stu-id="0393b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflow-from-identitycontainer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0393b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0393b-139">Response</span></span>

<span data-ttu-id="0393b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0393b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0393b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0393b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


