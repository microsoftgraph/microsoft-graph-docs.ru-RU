---
title: 'Пользователь: Чеккмемберобжектс'
description: Проверка членства в списке объектов группы, роли каталога или административных единиц для указанного объекта пользователя.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 118b8e95c9e5ef7d67d4e1b7792a5a7e4e39a193
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041751"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="6c30f-103">Пользователь: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="6c30f-103">user: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c30f-104">Проверка членства в списке объектов группы, роли каталога или административных единиц для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c30f-104">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="6c30f-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="6c30f-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c30f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c30f-106">Permissions</span></span>

<span data-ttu-id="6c30f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c30f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c30f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c30f-109">Permission type</span></span>                        | <span data-ttu-id="6c30f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c30f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c30f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c30f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c30f-112">User. ReadBasic, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="6c30f-113">Кроме того:</span><span class="sxs-lookup"><span data-stu-id="6c30f-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="6c30f-114">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="6c30f-115">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="6c30f-116">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="6c30f-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="6c30f-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c30f-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="6c30f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c30f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c30f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c30f-119">Not supported.</span></span> |
| <span data-ttu-id="6c30f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c30f-120">Application</span></span>                            | <span data-ttu-id="6c30f-121">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="6c30f-122">С</span><span class="sxs-lookup"><span data-stu-id="6c30f-122">And:</span></span><ul><li><span data-ttu-id="6c30f-123">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="6c30f-124">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c30f-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="6c30f-125">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="6c30f-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="6c30f-126">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c30f-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c30f-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c30f-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="6c30f-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c30f-128">Request headers</span></span>

| <span data-ttu-id="6c30f-129">Имя</span><span class="sxs-lookup"><span data-stu-id="6c30f-129">Name</span></span>          | <span data-ttu-id="6c30f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6c30f-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6c30f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c30f-131">Authorization</span></span> | <span data-ttu-id="6c30f-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6c30f-132">Bearer {token}</span></span> |
| <span data-ttu-id="6c30f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c30f-133">Content-Type</span></span>  | <span data-ttu-id="6c30f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6c30f-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c30f-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c30f-135">Request body</span></span>

<span data-ttu-id="6c30f-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6c30f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c30f-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c30f-137">Parameter</span></span>    | <span data-ttu-id="6c30f-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6c30f-138">Type</span></span>        | <span data-ttu-id="6c30f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6c30f-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c30f-140">ids</span><span class="sxs-lookup"><span data-stu-id="6c30f-140">ids</span></span>|<span data-ttu-id="6c30f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c30f-141">String collection</span></span>|<span data-ttu-id="6c30f-142">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="6c30f-142">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="6c30f-143">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="6c30f-143">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="6c30f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c30f-144">Response</span></span>

<span data-ttu-id="6c30f-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c30f-145">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c30f-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c30f-146">Examples</span></span>

<span data-ttu-id="6c30f-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6c30f-147">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6c30f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c30f-148">Request</span></span>

<span data-ttu-id="6c30f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c30f-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c30f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c30f-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c30f-151">C#</span><span class="sxs-lookup"><span data-stu-id="6c30f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c30f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c30f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c30f-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6c30f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c30f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c30f-154">Response</span></span>

<span data-ttu-id="6c30f-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c30f-155">The following is an example of the response.</span></span> 

><span data-ttu-id="6c30f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c30f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
