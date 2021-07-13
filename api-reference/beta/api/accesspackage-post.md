---
title: Создание accessPackage
description: Создание нового accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ccbe9c22f04087431ba0b4ae4df53eca1ff76a04
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400959"
---
# <a name="create-accesspackage"></a><span data-ttu-id="ee801-103">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="ee801-103">Create accessPackage</span></span>

<span data-ttu-id="ee801-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee801-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee801-105">Создайте новый [объект accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="ee801-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="ee801-106">Пакет доступа будет добавлен в существующий [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="ee801-106">The access package will be added to an existing [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="ee801-107">После создания пакета доступа можно создать [accessPackageAssignmentPolicies,](../resources/accesspackageassignmentpolicy.md) в которых указывается, как пользователи назначены пакету доступа.</span><span class="sxs-lookup"><span data-stu-id="ee801-107">After the access package is created, you can then create [accessPackageAssignmentPolicies](../resources/accesspackageassignmentpolicy.md) which specify how users are assigned to the access package.</span></span>


## <a name="permissions"></a><span data-ttu-id="ee801-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee801-108">Permissions</span></span>

<span data-ttu-id="ee801-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee801-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee801-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee801-111">Permission type</span></span>                        | <span data-ttu-id="ee801-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee801-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ee801-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee801-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee801-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee801-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ee801-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee801-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee801-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee801-116">Not supported.</span></span> |
| <span data-ttu-id="ee801-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ee801-117">Application</span></span>                            | <span data-ttu-id="ee801-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee801-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee801-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee801-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="ee801-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee801-120">Request headers</span></span>

| <span data-ttu-id="ee801-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ee801-121">Name</span></span>          | <span data-ttu-id="ee801-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ee801-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ee801-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee801-123">Authorization</span></span> | <span data-ttu-id="ee801-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee801-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="ee801-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee801-126">Content-type</span></span>  | <span data-ttu-id="ee801-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee801-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee801-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee801-129">Request body</span></span>

<span data-ttu-id="ee801-130">В теле запроса поставляем представление JSON объекта [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="ee801-130">In the request body, supply a JSON representation of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ee801-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee801-131">Response</span></span>

<span data-ttu-id="ee801-132">В случае успешной работы этот метод возвращает созданный код ответа 201 и новый [объект accessPackage](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee801-132">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee801-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ee801-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee801-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee801-134">Request</span></span>

<span data-ttu-id="ee801-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee801-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee801-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee801-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee801-137">C#</span><span class="sxs-lookup"><span data-stu-id="ee801-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee801-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee801-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee801-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee801-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee801-140">Java</span><span class="sxs-lookup"><span data-stu-id="ee801-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee801-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee801-141">Response</span></span>

<span data-ttu-id="ee801-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee801-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ee801-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee801-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


