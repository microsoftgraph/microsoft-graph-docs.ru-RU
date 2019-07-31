---
title: Удаление объекта Скопедролемембер
description: Удаление члена с областью ролей из единицы админстративе.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9321343e797bd45ca98ce470018481a7014684fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945888"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="27979-103">Удаление объекта Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="27979-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27979-104">Удаление члена с областью ролей из единицы админстративе.</span><span class="sxs-lookup"><span data-stu-id="27979-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="27979-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27979-105">Permissions</span></span>
<span data-ttu-id="27979-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27979-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27979-108">Permission type</span></span>      | <span data-ttu-id="27979-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27979-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27979-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27979-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27979-111">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="27979-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27979-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27979-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27979-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27979-113">Not supported.</span></span>    |
|<span data-ttu-id="27979-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27979-114">Application</span></span> | <span data-ttu-id="27979-115">Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="27979-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="27979-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27979-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="27979-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27979-117">Request headers</span></span>
| <span data-ttu-id="27979-118">Имя</span><span class="sxs-lookup"><span data-stu-id="27979-118">Name</span></span>       | <span data-ttu-id="27979-119">Описание</span><span class="sxs-lookup"><span data-stu-id="27979-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27979-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27979-120">Authorization</span></span>  | <span data-ttu-id="27979-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27979-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27979-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27979-123">Request body</span></span>
<span data-ttu-id="27979-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27979-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27979-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="27979-125">Response</span></span>

<span data-ttu-id="27979-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="27979-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27979-128">Пример</span><span class="sxs-lookup"><span data-stu-id="27979-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27979-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="27979-129">Request</span></span>
<span data-ttu-id="27979-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27979-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27979-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="27979-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27979-132">C#</span><span class="sxs-lookup"><span data-stu-id="27979-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27979-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="27979-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27979-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="27979-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27979-135">Java</span><span class="sxs-lookup"><span data-stu-id="27979-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27979-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="27979-136">Response</span></span>
<span data-ttu-id="27979-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27979-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
