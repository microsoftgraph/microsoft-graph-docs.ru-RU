---
title: Добавление элемента Скопедролемембер
description: Добавление нового Scopedrolemembership изменен. Примечание. в настоящее время поддерживаются только роли администраторов *учетных записей* и *администраторов службы технической поддержки* для членства в пределах ролей.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b48cdb0e6431a48c3227fd5996f9a17dc57fb291
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223447"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="03d9f-104">Добавление элемента Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="03d9f-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="03d9f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03d9f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03d9f-106">Добавление нового [scopedrolemembership изменен](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="03d9f-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="03d9f-107">Примечание. в настоящее время поддерживаются только роли администраторов *учетных записей* и *администраторов службы технической поддержки* для членства в пределах ролей.</span><span class="sxs-lookup"><span data-stu-id="03d9f-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="03d9f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03d9f-108">Permissions</span></span>
<span data-ttu-id="03d9f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03d9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="03d9f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03d9f-111">Permission type</span></span>      | <span data-ttu-id="03d9f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03d9f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03d9f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03d9f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="03d9f-114">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="03d9f-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03d9f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03d9f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03d9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d9f-116">Not supported.</span></span>    |
|<span data-ttu-id="03d9f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03d9f-117">Application</span></span> | <span data-ttu-id="03d9f-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="03d9f-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="03d9f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03d9f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="03d9f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03d9f-120">Request headers</span></span>
| <span data-ttu-id="03d9f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="03d9f-121">Name</span></span>      |<span data-ttu-id="03d9f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03d9f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03d9f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03d9f-123">Authorization</span></span>  | <span data-ttu-id="03d9f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03d9f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03d9f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03d9f-126">Request body</span></span>
<span data-ttu-id="03d9f-127">В тексте запроса добавьте представление объекта [scopedrolemembership изменен](../resources/scopedrolemembership.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03d9f-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03d9f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d9f-128">Response</span></span>

<span data-ttu-id="03d9f-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03d9f-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03d9f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="03d9f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03d9f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d9f-131">Request</span></span>
<span data-ttu-id="03d9f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03d9f-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03d9f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="03d9f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="03d9f-134">C#</span><span class="sxs-lookup"><span data-stu-id="03d9f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03d9f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03d9f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03d9f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03d9f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03d9f-137">Java</span><span class="sxs-lookup"><span data-stu-id="03d9f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

<span data-ttu-id="03d9f-138">В тексте запроса добавьте представление объекта [scopedrolemembership изменен](../resources/scopedrolemembership.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03d9f-138">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03d9f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d9f-139">Response</span></span>
<span data-ttu-id="03d9f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03d9f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#scopedRoleMemberships/$entity",
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
