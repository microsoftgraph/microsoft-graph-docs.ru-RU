---
title: Создание Акцесспаккаже
description: Создание нового Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef57e5400d2bb93bf566badfc76fa8c890206809
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448511"
---
# <a name="create-accesspackage"></a><span data-ttu-id="154fe-103">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="154fe-103">Create accessPackage</span></span>

<span data-ttu-id="154fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="154fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="154fe-105">Создание нового объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="154fe-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="154fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="154fe-106">Permissions</span></span>

<span data-ttu-id="154fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="154fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="154fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="154fe-109">Permission type</span></span>                        | <span data-ttu-id="154fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="154fe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="154fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="154fe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="154fe-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154fe-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="154fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="154fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="154fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="154fe-114">Not supported.</span></span> |
| <span data-ttu-id="154fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="154fe-115">Application</span></span>                            | <span data-ttu-id="154fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="154fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="154fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="154fe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="154fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="154fe-118">Request headers</span></span>

| <span data-ttu-id="154fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="154fe-119">Name</span></span>          | <span data-ttu-id="154fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="154fe-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="154fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="154fe-121">Authorization</span></span> | <span data-ttu-id="154fe-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="154fe-122">Bearer \{token\}.</span></span> <span data-ttu-id="154fe-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="154fe-123">Required.</span></span> |
| <span data-ttu-id="154fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="154fe-124">Content-Type</span></span>  | <span data-ttu-id="154fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="154fe-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="154fe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="154fe-126">Request body</span></span>

<span data-ttu-id="154fe-127">В тексте запроса добавьте представление объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="154fe-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="154fe-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="154fe-128">Response</span></span>

<span data-ttu-id="154fe-129">В случае успешного выполнения этот метод возвращает код отклика 201, созданный в теле отклика, и новый объект [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="154fe-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="154fe-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="154fe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="154fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="154fe-131">Request</span></span>

<span data-ttu-id="154fe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="154fe-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="154fe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="154fe-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="154fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="154fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="154fe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="154fe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="154fe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="154fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="154fe-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="154fe-137">Response</span></span>

<span data-ttu-id="154fe-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="154fe-138">The following is an example of the response.</span></span>

> <span data-ttu-id="154fe-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="154fe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
