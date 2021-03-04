---
title: Добавление scopedRoleMember
description: Добавьте новое scopedRoleMembership. ПРИМЕЧАНИЕ. Только *роли* администратора учетной записи пользователя и *администратора Helpdesk* в настоящее время поддерживаются для членства в scoped-role.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7bf20ae9e7b18b5fc4ff1402fe8ac7538f9e4d86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438757"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="83aff-104">Добавление scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="83aff-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="83aff-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83aff-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83aff-106">Добавьте новое [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="83aff-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="83aff-107">ПРИМЕЧАНИЕ. Только *роли* администратора учетной записи пользователя и *администратора Helpdesk* в настоящее время поддерживаются для членства в scoped-role.</span><span class="sxs-lookup"><span data-stu-id="83aff-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="83aff-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83aff-108">Permissions</span></span>
<span data-ttu-id="83aff-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83aff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83aff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83aff-111">Permission type</span></span>      | <span data-ttu-id="83aff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83aff-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83aff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83aff-113">Delegated (work or school account)</span></span> | <span data-ttu-id="83aff-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83aff-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83aff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83aff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83aff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83aff-116">Not supported.</span></span>    |
|<span data-ttu-id="83aff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="83aff-117">Application</span></span> | <span data-ttu-id="83aff-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="83aff-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="83aff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83aff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="83aff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83aff-120">Request headers</span></span>
| <span data-ttu-id="83aff-121">Имя</span><span class="sxs-lookup"><span data-stu-id="83aff-121">Name</span></span>      |<span data-ttu-id="83aff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="83aff-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83aff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83aff-123">Authorization</span></span>  | <span data-ttu-id="83aff-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83aff-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83aff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83aff-126">Request body</span></span>
<span data-ttu-id="83aff-127">В теле запроса поставляют представление JSON объекта [scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="83aff-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83aff-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="83aff-128">Response</span></span>

<span data-ttu-id="83aff-129">В случае успешного применения этот метод возвращает код ответа и `201 Created` [объект scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="83aff-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83aff-130">Пример</span><span class="sxs-lookup"><span data-stu-id="83aff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83aff-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="83aff-131">Request</span></span>
<span data-ttu-id="83aff-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83aff-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83aff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="83aff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="83aff-134">C#</span><span class="sxs-lookup"><span data-stu-id="83aff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83aff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83aff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83aff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83aff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83aff-137">Java</span><span class="sxs-lookup"><span data-stu-id="83aff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="83aff-138">В теле запроса поставляют представление JSON объекта [scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="83aff-138">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="83aff-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="83aff-139">Response</span></span>
<span data-ttu-id="83aff-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83aff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


