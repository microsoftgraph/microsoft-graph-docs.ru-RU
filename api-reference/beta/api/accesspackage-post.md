---
title: Создание accessPackage
description: Создание нового accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1a415978968b4fa03133de156702ead1c473f1a1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439774"
---
# <a name="create-accesspackage"></a><span data-ttu-id="8c685-103">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="8c685-103">Create accessPackage</span></span>

<span data-ttu-id="8c685-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c685-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c685-105">Создайте новый [объект accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8c685-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c685-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c685-106">Permissions</span></span>

<span data-ttu-id="8c685-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c685-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c685-109">Permission type</span></span>                        | <span data-ttu-id="8c685-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c685-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c685-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c685-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c685-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c685-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8c685-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c685-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c685-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c685-114">Not supported.</span></span> |
| <span data-ttu-id="8c685-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c685-115">Application</span></span>                            | <span data-ttu-id="8c685-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c685-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c685-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c685-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="8c685-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c685-118">Request headers</span></span>

| <span data-ttu-id="8c685-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8c685-119">Name</span></span>          | <span data-ttu-id="8c685-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c685-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8c685-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c685-121">Authorization</span></span> | <span data-ttu-id="8c685-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="8c685-122">Bearer \{token\}.</span></span> <span data-ttu-id="8c685-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8c685-123">Required.</span></span> |
| <span data-ttu-id="8c685-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c685-124">Content-Type</span></span>  | <span data-ttu-id="8c685-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c685-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c685-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c685-126">Request body</span></span>

<span data-ttu-id="8c685-127">В теле запроса поставляем JSON-представление [объекта accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8c685-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8c685-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c685-128">Response</span></span>

<span data-ttu-id="8c685-129">В случае успешной работы этот метод возвращает созданный код ответа 201 и новый [объект accessPackage](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c685-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c685-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c685-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c685-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c685-131">Request</span></span>

<span data-ttu-id="8c685-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c685-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c685-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c685-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```
# <a name="c"></a>[<span data-ttu-id="8c685-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c685-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c685-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c685-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c685-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c685-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c685-137">Java</span><span class="sxs-lookup"><span data-stu-id="8c685-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c685-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c685-138">Response</span></span>

<span data-ttu-id="8c685-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c685-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8c685-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c685-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


