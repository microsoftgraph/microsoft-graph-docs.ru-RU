---
title: 'Пользователь: Чеккмемберобжектс'
description: Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a33da99187ba8d8bbc64ea119dd3c3a13491a92e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108412"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="42d89-103">Пользователь: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="42d89-103">user: checkMemberObjects</span></span>

<span data-ttu-id="42d89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42d89-105">Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="42d89-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="42d89-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="42d89-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="42d89-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42d89-107">Permissions</span></span>

<span data-ttu-id="42d89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42d89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42d89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42d89-110">Permission type</span></span>                        | <span data-ttu-id="42d89-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42d89-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42d89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42d89-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="42d89-113">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="42d89-114">Дополнительно:</span><span class="sxs-lookup"><span data-stu-id="42d89-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="42d89-115">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="42d89-116">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="42d89-117">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="42d89-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="42d89-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42d89-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="42d89-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42d89-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42d89-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42d89-120">Not supported.</span></span> |
| <span data-ttu-id="42d89-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42d89-121">Application</span></span>                            | <span data-ttu-id="42d89-122">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="42d89-123">С</span><span class="sxs-lookup"><span data-stu-id="42d89-123">And:</span></span><ul><li><span data-ttu-id="42d89-124">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="42d89-125">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42d89-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="42d89-126">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="42d89-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="42d89-127">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d89-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42d89-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42d89-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="42d89-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42d89-129">Request headers</span></span>

| <span data-ttu-id="42d89-130">Имя</span><span class="sxs-lookup"><span data-stu-id="42d89-130">Name</span></span>          | <span data-ttu-id="42d89-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42d89-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="42d89-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42d89-132">Authorization</span></span> | <span data-ttu-id="42d89-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42d89-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42d89-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42d89-135">Content-Type</span></span>  | <span data-ttu-id="42d89-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42d89-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42d89-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42d89-138">Request body</span></span>

<span data-ttu-id="42d89-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="42d89-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42d89-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="42d89-140">Parameter</span></span>    | <span data-ttu-id="42d89-141">Тип</span><span class="sxs-lookup"><span data-stu-id="42d89-141">Type</span></span>        | <span data-ttu-id="42d89-142">Описание</span><span class="sxs-lookup"><span data-stu-id="42d89-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42d89-143">ids</span><span class="sxs-lookup"><span data-stu-id="42d89-143">ids</span></span>|<span data-ttu-id="42d89-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42d89-144">String collection</span></span>|<span data-ttu-id="42d89-145">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="42d89-145">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="42d89-146">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="42d89-146">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="42d89-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="42d89-147">Response</span></span>

<span data-ttu-id="42d89-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42d89-148">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42d89-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="42d89-149">Examples</span></span>

<span data-ttu-id="42d89-150">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="42d89-150">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="42d89-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="42d89-151">Request</span></span>

<span data-ttu-id="42d89-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42d89-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42d89-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="42d89-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="42d89-154">C#</span><span class="sxs-lookup"><span data-stu-id="42d89-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42d89-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42d89-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42d89-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42d89-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42d89-157">Java</span><span class="sxs-lookup"><span data-stu-id="42d89-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42d89-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="42d89-158">Response</span></span>

<span data-ttu-id="42d89-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42d89-159">The following is an example of the response.</span></span> 

><span data-ttu-id="42d89-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42d89-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
