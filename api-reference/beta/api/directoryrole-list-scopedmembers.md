---
title: Список scopedMembers для роли каталога
description: Извлечение списка объектов scopedRoleMembership для роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a9a905ddc0f645f792603d4afbde3eb79b0d017
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53119179"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="a89be-103">Список scopedMembers для роли каталога</span><span class="sxs-lookup"><span data-stu-id="a89be-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="a89be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89be-105">Извлечение списка [объектов scopedRoleMembership](../resources/scopedrolemembership.md) для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a89be-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="a89be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89be-106">Permissions</span></span>
<span data-ttu-id="a89be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89be-109">Permission type</span></span>      | <span data-ttu-id="a89be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a89be-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a89be-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a89be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89be-114">Not supported.</span></span>    |
|<span data-ttu-id="a89be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89be-115">Application</span></span> | <span data-ttu-id="a89be-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89be-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{role-id}/scopedMembers
GET /directoryroles/roleTemplateId={roleTemplateId}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a89be-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a89be-118">Optional query parameters</span></span>
<span data-ttu-id="a89be-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a89be-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a89be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89be-120">Request headers</span></span>
| <span data-ttu-id="a89be-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a89be-121">Name</span></span>      |<span data-ttu-id="a89be-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a89be-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a89be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89be-123">Authorization</span></span>  | <span data-ttu-id="a89be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a89be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a89be-126">Request body</span></span>
<span data-ttu-id="a89be-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a89be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89be-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89be-128">Response</span></span>

<span data-ttu-id="a89be-129">В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a89be-129">If successful, this method returns a `200 OK` response code and a collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="a89be-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a89be-130">Examples</span></span>

### <a name="example-1--get-the-scoped-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="a89be-131">Пример 1. Получить масштабные члены роли каталога с помощью role id</span><span class="sxs-lookup"><span data-stu-id="a89be-131">Example 1:  Get the scoped members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89be-132">Request</span></span>
<span data-ttu-id="a89be-133">Ниже приводится пример запроса на id роли **каталога** `41d12a2f-caa8-4e3e-ba14-05e5102ce085` .</span><span class="sxs-lookup"><span data-stu-id="a89be-133">The following is an example of a request for a directory role **id** `41d12a2f-caa8-4e3e-ba14-05e5102ce085`.</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="a89be-135">C#</span><span class="sxs-lookup"><span data-stu-id="a89be-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a89be-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a89be-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a89be-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a89be-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a89be-138">Java</span><span class="sxs-lookup"><span data-stu-id="a89be-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a89be-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89be-139">Response</span></span>
<span data-ttu-id="a89be-140">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a89be-140">The following example shows the response.</span></span> 
><span data-ttu-id="a89be-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a89be-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

### <a name="example-2--get-the-scoped-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="a89be-142">Пример 2. Получить масштабные члены роли каталога с помощью roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a89be-142">Example 2:  Get the scoped members of a directory role using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89be-143">Request</span></span>
<span data-ttu-id="a89be-144">Ниже приводится пример запроса на роль каталога с **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c` .</span><span class="sxs-lookup"><span data-stu-id="a89be-144">The following is an example of a request for a directory role with **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers
```

#### <a name="response"></a><span data-ttu-id="a89be-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89be-145">Response</span></span>
<span data-ttu-id="a89be-146">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a89be-146">The following example shows the response.</span></span> 
><span data-ttu-id="a89be-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a89be-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
