---
title: Удаление объекта Скопедролемембер
description: Удаление члена с областью ролей из единицы админстративе.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9860f82bcd186ab9863685f75f7d75c3bfbf4ff8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962724"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="c80e2-103">Удаление объекта Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="c80e2-103">Remove a scopedRoleMember</span></span>

<span data-ttu-id="c80e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c80e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c80e2-105">Удаление члена с областью ролей из единицы админстративе.</span><span class="sxs-lookup"><span data-stu-id="c80e2-105">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="c80e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c80e2-106">Permissions</span></span>
<span data-ttu-id="c80e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c80e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c80e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c80e2-109">Permission type</span></span>      | <span data-ttu-id="c80e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c80e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c80e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c80e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c80e2-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c80e2-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c80e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c80e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c80e2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c80e2-114">Not supported.</span></span>    |
|<span data-ttu-id="c80e2-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c80e2-115">Application</span></span> | <span data-ttu-id="c80e2-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="c80e2-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c80e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c80e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c80e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c80e2-118">Request headers</span></span>
| <span data-ttu-id="c80e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c80e2-119">Name</span></span>       | <span data-ttu-id="c80e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c80e2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c80e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c80e2-121">Authorization</span></span>  | <span data-ttu-id="c80e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c80e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c80e2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c80e2-124">Request body</span></span>
<span data-ttu-id="c80e2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c80e2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c80e2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80e2-126">Response</span></span>

<span data-ttu-id="c80e2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c80e2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c80e2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c80e2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c80e2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c80e2-130">Request</span></span>
<span data-ttu-id="c80e2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c80e2-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c80e2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c80e2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="c80e2-133">C#</span><span class="sxs-lookup"><span data-stu-id="c80e2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c80e2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c80e2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c80e2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c80e2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c80e2-136">Java</span><span class="sxs-lookup"><span data-stu-id="c80e2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c80e2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80e2-137">Response</span></span>
<span data-ttu-id="c80e2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c80e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


