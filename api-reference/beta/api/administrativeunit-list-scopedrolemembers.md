---
title: Список Scopedadministrators
description: Получение списка ресурсов Scopedrolemembership изменен.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbcdecdc227477dc53c137547c0e78b46b92107d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123358"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="3ec81-103">Список Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="3ec81-103">List scopedRoleMembers</span></span>

<span data-ttu-id="3ec81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec81-105">Получение списка ресурсов [scopedrolemembership изменен](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="3ec81-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ec81-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec81-106">Permissions</span></span>
<span data-ttu-id="3ec81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ec81-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec81-109">Permission type</span></span>      | <span data-ttu-id="3ec81-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec81-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ec81-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec81-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec81-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="3ec81-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ec81-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec81-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec81-114">Not supported.</span></span>    |
|<span data-ttu-id="3ec81-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ec81-115">Application</span></span> | <span data-ttu-id="3ec81-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ec81-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec81-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec81-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ec81-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ec81-118">Optional query parameters</span></span>
<span data-ttu-id="3ec81-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3ec81-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ec81-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ec81-120">Request headers</span></span>
| <span data-ttu-id="3ec81-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3ec81-121">Name</span></span>      |<span data-ttu-id="3ec81-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec81-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ec81-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ec81-123">Authorization</span></span>  | <span data-ttu-id="3ec81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ec81-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec81-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ec81-126">Request body</span></span>
<span data-ttu-id="3ec81-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ec81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec81-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ec81-128">Response</span></span>

<span data-ttu-id="3ec81-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec81-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ec81-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ec81-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ec81-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec81-131">Request</span></span>
<span data-ttu-id="3ec81-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ec81-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ec81-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec81-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="c"></a>[<span data-ttu-id="3ec81-134">C#</span><span class="sxs-lookup"><span data-stu-id="3ec81-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec81-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec81-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec81-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec81-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3ec81-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec81-137">Response</span></span>
<span data-ttu-id="3ec81-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ec81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
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
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
