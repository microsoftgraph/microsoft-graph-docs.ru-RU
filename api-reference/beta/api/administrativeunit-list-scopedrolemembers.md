---
title: Список Scopedadministrators
description: Получение списка ресурсов Scopedrolemembership изменен.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83eb193d46b6ee206beb3c86404e35fb8ed10cad
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917963"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="b0ba6-103">Список Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="b0ba6-103">List scopedRoleMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ba6-104">Получение списка ресурсов [scopedrolemembership изменен](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="b0ba6-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0ba6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0ba6-105">Permissions</span></span>
<span data-ttu-id="b0ba6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0ba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0ba6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0ba6-108">Permission type</span></span>      | <span data-ttu-id="b0ba6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0ba6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ba6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0ba6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ba6-111">AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b0ba6-111">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0ba6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0ba6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ba6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-113">Not supported.</span></span>    |
|<span data-ttu-id="b0ba6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0ba6-114">Application</span></span> | <span data-ttu-id="b0ba6-115">AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0ba6-115">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ba6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0ba6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0ba6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0ba6-117">Optional query parameters</span></span>
<span data-ttu-id="b0ba6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0ba6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0ba6-119">Request headers</span></span>
| <span data-ttu-id="b0ba6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b0ba6-120">Name</span></span>      |<span data-ttu-id="b0ba6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b0ba6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0ba6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0ba6-122">Authorization</span></span>  | <span data-ttu-id="b0ba6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0ba6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0ba6-125">Request body</span></span>
<span data-ttu-id="b0ba6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0ba6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0ba6-127">Response</span></span>

<span data-ttu-id="b0ba6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0ba6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b0ba6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0ba6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0ba6-130">Request</span></span>
<span data-ttu-id="b0ba6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0ba6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0ba6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0ba6-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0ba6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0ba6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0ba6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0ba6-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0ba6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0ba6-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0ba6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0ba6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0ba6-137">Response</span></span>
<span data-ttu-id="b0ba6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0ba6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
