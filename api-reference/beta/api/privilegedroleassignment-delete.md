---
title: Удаление privilegedRoleAssignment
description: Удаление Привилежедролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 76db67452db136d126774f2b7c93e372e7e582f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444997"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="44769-103">Удаление privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="44769-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44769-104">Удаление [привилежедролеассигнмент](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="44769-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="44769-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44769-105">Permissions</span></span>
<span data-ttu-id="44769-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="44769-108">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="44769-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="44769-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44769-109">Permission type</span></span>      | <span data-ttu-id="44769-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44769-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44769-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44769-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44769-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44769-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44769-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44769-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44769-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44769-114">Not supported.</span></span>    |
|<span data-ttu-id="44769-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44769-115">Application</span></span> | <span data-ttu-id="44769-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44769-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44769-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44769-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="44769-118">Обратите ``<id>`` внимание, что в формате "усерид_ролеид", где UserID — это строка GUID для идентификатора пользователя Azure AD, а roleId — строка GUID для идентификатора роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="44769-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44769-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44769-119">Request headers</span></span>
| <span data-ttu-id="44769-120">Имя</span><span class="sxs-lookup"><span data-stu-id="44769-120">Name</span></span>       | <span data-ttu-id="44769-121">Описание</span><span class="sxs-lookup"><span data-stu-id="44769-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44769-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44769-122">Authorization</span></span>  | <span data-ttu-id="44769-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44769-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44769-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44769-125">Request body</span></span>
<span data-ttu-id="44769-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44769-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44769-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="44769-127">Response</span></span>

<span data-ttu-id="44769-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="44769-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="44769-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="44769-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="44769-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="44769-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="44769-132">Пример</span><span class="sxs-lookup"><span data-stu-id="44769-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44769-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="44769-133">Request</span></span>
<span data-ttu-id="44769-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44769-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44769-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="44769-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44769-136">C#</span><span class="sxs-lookup"><span data-stu-id="44769-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44769-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="44769-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44769-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="44769-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44769-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="44769-139">Response</span></span>
<span data-ttu-id="44769-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44769-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
