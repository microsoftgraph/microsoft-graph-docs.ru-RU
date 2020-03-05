---
title: Удаление объекта Скопедролемембер
description: Удаление члена с областью ролей из единицы админстративе.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2353ab7a956748f1284e2bd27ea5a1101359b8fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441767"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="d9130-103">Удаление объекта Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="d9130-103">Remove a scopedRoleMember</span></span>

<span data-ttu-id="d9130-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9130-105">Удаление члена с областью ролей из единицы админстративе.</span><span class="sxs-lookup"><span data-stu-id="d9130-105">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9130-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9130-106">Permissions</span></span>
<span data-ttu-id="d9130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9130-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9130-109">Permission type</span></span>      | <span data-ttu-id="d9130-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9130-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9130-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9130-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9130-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d9130-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9130-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9130-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9130-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9130-114">Not supported.</span></span>    |
|<span data-ttu-id="d9130-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9130-115">Application</span></span> | <span data-ttu-id="d9130-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d9130-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9130-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9130-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d9130-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9130-118">Request headers</span></span>
| <span data-ttu-id="d9130-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d9130-119">Name</span></span>       | <span data-ttu-id="d9130-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9130-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9130-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9130-121">Authorization</span></span>  | <span data-ttu-id="d9130-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9130-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9130-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9130-124">Request body</span></span>
<span data-ttu-id="d9130-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9130-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9130-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9130-126">Response</span></span>

<span data-ttu-id="d9130-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9130-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9130-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d9130-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9130-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9130-130">Request</span></span>
<span data-ttu-id="d9130-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9130-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9130-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9130-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="d9130-133">C#</span><span class="sxs-lookup"><span data-stu-id="d9130-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9130-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9130-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9130-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9130-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9130-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9130-136">Response</span></span>
<span data-ttu-id="d9130-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9130-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
