---
title: 'Пользователь: Чеккмемберобжектс'
description: Проверка членства в списке объектов группы, роли каталога или административных единиц для указанного объекта пользователя.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 31f5d772002516a267bac68fa0f1f7434b6810e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452017"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="511d0-103">Пользователь: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="511d0-103">user: checkMemberObjects</span></span>

<span data-ttu-id="511d0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="511d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="511d0-105">Проверка членства в списке объектов группы, роли каталога или административных единиц для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="511d0-105">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="511d0-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="511d0-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="511d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="511d0-107">Permissions</span></span>

<span data-ttu-id="511d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="511d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="511d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="511d0-110">Permission type</span></span>                        | <span data-ttu-id="511d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="511d0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="511d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="511d0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="511d0-113">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="511d0-114">Дополнительно:</span><span class="sxs-lookup"><span data-stu-id="511d0-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="511d0-115">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="511d0-116">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="511d0-117">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="511d0-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="511d0-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="511d0-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="511d0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="511d0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="511d0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511d0-120">Not supported.</span></span> |
| <span data-ttu-id="511d0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="511d0-121">Application</span></span>                            | <span data-ttu-id="511d0-122">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="511d0-123">С</span><span class="sxs-lookup"><span data-stu-id="511d0-123">And:</span></span><ul><li><span data-ttu-id="511d0-124">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="511d0-125">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="511d0-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="511d0-126">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="511d0-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="511d0-127">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="511d0-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="511d0-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="511d0-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="511d0-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="511d0-129">Request headers</span></span>

| <span data-ttu-id="511d0-130">Имя</span><span class="sxs-lookup"><span data-stu-id="511d0-130">Name</span></span>          | <span data-ttu-id="511d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="511d0-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="511d0-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="511d0-132">Authorization</span></span> | <span data-ttu-id="511d0-133">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="511d0-133">Bearer {token}</span></span> |
| <span data-ttu-id="511d0-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="511d0-134">Content-Type</span></span>  | <span data-ttu-id="511d0-135">application/json</span><span class="sxs-lookup"><span data-stu-id="511d0-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="511d0-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="511d0-136">Request body</span></span>

<span data-ttu-id="511d0-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="511d0-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="511d0-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="511d0-138">Parameter</span></span>    | <span data-ttu-id="511d0-139">Тип</span><span class="sxs-lookup"><span data-stu-id="511d0-139">Type</span></span>        | <span data-ttu-id="511d0-140">Описание</span><span class="sxs-lookup"><span data-stu-id="511d0-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="511d0-141">ids</span><span class="sxs-lookup"><span data-stu-id="511d0-141">ids</span></span>|<span data-ttu-id="511d0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="511d0-142">String collection</span></span>|<span data-ttu-id="511d0-143">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="511d0-143">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="511d0-144">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="511d0-144">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="511d0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="511d0-145">Response</span></span>

<span data-ttu-id="511d0-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="511d0-146">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="511d0-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="511d0-147">Examples</span></span>

<span data-ttu-id="511d0-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="511d0-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="511d0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="511d0-149">Request</span></span>

<span data-ttu-id="511d0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="511d0-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="511d0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="511d0-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="511d0-152">C#</span><span class="sxs-lookup"><span data-stu-id="511d0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="511d0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="511d0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="511d0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="511d0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="511d0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="511d0-155">Response</span></span>

<span data-ttu-id="511d0-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="511d0-156">The following is an example of the response.</span></span> 

><span data-ttu-id="511d0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="511d0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
