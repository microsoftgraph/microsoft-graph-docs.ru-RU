---
title: Добавление элемента Скопедролемембер
description: Добавление нового Scopedrolemembership изменен. Примечание. в настоящее время поддерживаются только роли администраторов *учетных записей* и *администраторов службы технической поддержки* для членства в пределах ролей.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56bd18794a6e138b537524f63f4f1fc5cac483bc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962528"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="8da06-104">Добавление элемента Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="8da06-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="8da06-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da06-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da06-106">Добавление нового [scopedrolemembership изменен](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="8da06-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="8da06-107">Примечание. в настоящее время поддерживаются только роли администраторов *учетных записей* и *администраторов службы технической поддержки* для членства в пределах ролей.</span><span class="sxs-lookup"><span data-stu-id="8da06-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da06-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8da06-108">Permissions</span></span>
<span data-ttu-id="8da06-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8da06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8da06-111">Permission type</span></span>      | <span data-ttu-id="8da06-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8da06-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8da06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8da06-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8da06-114">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8da06-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8da06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8da06-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da06-116">Not supported.</span></span>    |
|<span data-ttu-id="8da06-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8da06-117">Application</span></span> | <span data-ttu-id="8da06-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="8da06-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="8da06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8da06-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="8da06-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8da06-120">Request headers</span></span>
| <span data-ttu-id="8da06-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8da06-121">Name</span></span>      |<span data-ttu-id="8da06-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8da06-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8da06-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8da06-123">Authorization</span></span>  | <span data-ttu-id="8da06-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8da06-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da06-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8da06-126">Request body</span></span>
<span data-ttu-id="8da06-127">В тексте запроса добавьте представление объекта [scopedrolemembership изменен](../resources/scopedrolemembership.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8da06-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8da06-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da06-128">Response</span></span>

<span data-ttu-id="8da06-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8da06-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da06-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8da06-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8da06-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8da06-131">Request</span></span>
<span data-ttu-id="8da06-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8da06-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8da06-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8da06-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8da06-134">C#</span><span class="sxs-lookup"><span data-stu-id="8da06-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8da06-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8da06-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8da06-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8da06-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8da06-137">Java</span><span class="sxs-lookup"><span data-stu-id="8da06-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8da06-138">В тексте запроса добавьте представление объекта [scopedrolemembership изменен](../resources/scopedrolemembership.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8da06-138">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8da06-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da06-139">Response</span></span>
<span data-ttu-id="8da06-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8da06-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


