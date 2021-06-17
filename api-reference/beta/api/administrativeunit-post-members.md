---
title: Добавление участника
description: Используйте этот API для добавления участника (пользователя или группы) в административное подразделение.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 46bd9fee6ca7353132fb9bc16183093a7a5dd465
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991941"
---
# <a name="add-a-member"></a><span data-ttu-id="119be-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="119be-103">Add a member</span></span>

<span data-ttu-id="119be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="119be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119be-105">Используйте этот API для добавления участника (пользователя или группы) в административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="119be-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="119be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="119be-106">Permissions</span></span>
<span data-ttu-id="119be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="119be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="119be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="119be-109">Permission type</span></span>      | <span data-ttu-id="119be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="119be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="119be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="119be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="119be-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="119be-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="119be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="119be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="119be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="119be-114">Not supported.</span></span>    |
|<span data-ttu-id="119be-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="119be-115">Application</span></span> | <span data-ttu-id="119be-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="119be-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="119be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="119be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="119be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="119be-118">Request headers</span></span>
| <span data-ttu-id="119be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="119be-119">Name</span></span>      |<span data-ttu-id="119be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="119be-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="119be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="119be-121">Authorization</span></span>  | <span data-ttu-id="119be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="119be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="119be-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="119be-124">Request body</span></span>
<span data-ttu-id="119be-125">В теле запроса укажи добавить пользователя, группу или `id` [directoryObject.](../resources/directoryobject.md) [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="119be-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="119be-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="119be-126">Response</span></span>

<span data-ttu-id="119be-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="119be-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="119be-129">Пример</span><span class="sxs-lookup"><span data-stu-id="119be-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="119be-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="119be-130">Request</span></span>
<span data-ttu-id="119be-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="119be-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="119be-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="119be-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="119be-133">C#</span><span class="sxs-lookup"><span data-stu-id="119be-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="119be-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="119be-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="119be-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="119be-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="119be-136">Java</span><span class="sxs-lookup"><span data-stu-id="119be-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="119be-137">В теле запроса укажи объект пользователя или группы, который `id` необходимо добавить. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="119be-137">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="119be-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="119be-138">Response</span></span>
<span data-ttu-id="119be-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="119be-139">Here is an example of the response.</span></span>
 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


