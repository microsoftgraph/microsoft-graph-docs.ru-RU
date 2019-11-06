---
title: Создание Акцесспаккаже
description: Создание нового Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a70de297dcd22588914d8613635687f07aaf40b0
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994130"
---
# <a name="create-accesspackage"></a><span data-ttu-id="ff5ac-103">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="ff5ac-103">Create accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff5ac-104">Создание нового объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="ff5ac-104">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff5ac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff5ac-105">Permissions</span></span>

<span data-ttu-id="ff5ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff5ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff5ac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff5ac-108">Permission type</span></span>                        | <span data-ttu-id="ff5ac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff5ac-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff5ac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff5ac-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff5ac-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5ac-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ff5ac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff5ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff5ac-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-113">Not supported.</span></span> |
| <span data-ttu-id="ff5ac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff5ac-114">Application</span></span>                            | <span data-ttu-id="ff5ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff5ac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff5ac-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="ff5ac-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff5ac-117">Request headers</span></span>

| <span data-ttu-id="ff5ac-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ff5ac-118">Name</span></span>          | <span data-ttu-id="ff5ac-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ff5ac-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff5ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff5ac-120">Authorization</span></span> | <span data-ttu-id="ff5ac-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-121">Bearer \{token\}.</span></span> <span data-ttu-id="ff5ac-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-122">Required.</span></span> |
| <span data-ttu-id="ff5ac-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff5ac-123">Content-Type</span></span>  | <span data-ttu-id="ff5ac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff5ac-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff5ac-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff5ac-125">Request body</span></span>

<span data-ttu-id="ff5ac-126">В тексте запроса добавьте представление объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-126">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ff5ac-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff5ac-127">Response</span></span>

<span data-ttu-id="ff5ac-128">В случае успешного выполнения этот метод возвращает код отклика 201, созданный в теле отклика, и новый объект [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="ff5ac-128">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff5ac-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff5ac-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff5ac-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff5ac-130">Request</span></span>

<span data-ttu-id="ff5ac-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff5ac-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff5ac-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff5ac-133">C#</span><span class="sxs-lookup"><span data-stu-id="ff5ac-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff5ac-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff5ac-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff5ac-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff5ac-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff5ac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff5ac-136">Response</span></span>

<span data-ttu-id="ff5ac-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ff5ac-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff5ac-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
