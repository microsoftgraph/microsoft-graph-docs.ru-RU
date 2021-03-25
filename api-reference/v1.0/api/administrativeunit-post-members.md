---
title: Добавление участника
description: Используйте этот API для добавления участника (пользователя или группы) в административное подразделение.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8fac296f9bf281a1ef3140f469dfd80f7c0a935b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202160"
---
# <a name="add-a-member"></a><span data-ttu-id="1b837-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="1b837-103">Add a member</span></span>

<span data-ttu-id="1b837-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b837-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b837-105">Используйте этот API для добавления участника (пользователя или группы) в административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="1b837-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="1b837-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b837-106">Permissions</span></span>
<span data-ttu-id="1b837-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1b837-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b837-109">Permission type</span></span>      | <span data-ttu-id="1b837-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b837-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b837-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b837-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b837-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b837-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b837-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b837-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b837-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b837-114">Not supported.</span></span>    |
|<span data-ttu-id="1b837-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b837-115">Application</span></span> | <span data-ttu-id="1b837-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b837-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b837-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b837-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1b837-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b837-118">Request headers</span></span>
| <span data-ttu-id="1b837-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1b837-119">Name</span></span>      |<span data-ttu-id="1b837-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b837-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b837-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b837-121">Authorization</span></span>  | <span data-ttu-id="1b837-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b837-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b837-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b837-124">Request body</span></span>
<span data-ttu-id="1b837-125">В теле запроса укажи добавить пользователя, группу или `id` [directoryObject.](../resources/directoryobject.md) [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="1b837-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="1b837-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b837-126">Response</span></span>

<span data-ttu-id="1b837-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1b837-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b837-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1b837-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b837-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b837-130">Request</span></span>
<span data-ttu-id="1b837-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b837-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b837-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b837-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/v1.0/groups/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="1b837-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b837-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b837-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b837-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b837-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b837-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b837-136">Java</span><span class="sxs-lookup"><span data-stu-id="1b837-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1b837-137">В теле запроса укажи объект пользователя или группы, который `id` необходимо добавить. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="1b837-137">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="1b837-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b837-138">Response</span></span>
<span data-ttu-id="1b837-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b837-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
