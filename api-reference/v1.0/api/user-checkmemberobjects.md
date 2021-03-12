---
title: 'пользователь: checkMemberObjects'
description: Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4f27a53030e1c01b3efb1967f9f0620033e36f28
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722393"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="8dd1c-103">пользователь: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8dd1c-103">user: checkMemberObjects</span></span>

<span data-ttu-id="8dd1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dd1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dd1c-105">Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="8dd1c-106">Этот метод является транзитным.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd1c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd1c-107">Permissions</span></span>

<span data-ttu-id="8dd1c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dd1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd1c-110">Permission type</span></span>                        | <span data-ttu-id="8dd1c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dd1c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dd1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dd1c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dd1c-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="8dd1c-114">Кроме того:</span><span class="sxs-lookup"><span data-stu-id="8dd1c-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="8dd1c-115">При проверке на членство в группах: Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="8dd1c-116">При проверке на членство в административных подразделениях: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="8dd1c-117">При проверке на членство в ролях каталога: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="8dd1c-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="8dd1c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="8dd1c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dd1c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dd1c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-120">Not supported.</span></span> |
| <span data-ttu-id="8dd1c-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dd1c-121">Application</span></span>                            | <span data-ttu-id="8dd1c-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="8dd1c-123">И:</span><span class="sxs-lookup"><span data-stu-id="8dd1c-123">And:</span></span><ul><li><span data-ttu-id="8dd1c-124">При проверке на членство в группах: Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="8dd1c-125">При проверке на членство в административных подразделениях: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="8dd1c-126">При проверке на членство в ролях каталога: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="8dd1c-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="8dd1c-127">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd1c-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dd1c-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dd1c-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="8dd1c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dd1c-129">Request headers</span></span>

| <span data-ttu-id="8dd1c-130">Имя</span><span class="sxs-lookup"><span data-stu-id="8dd1c-130">Name</span></span>          | <span data-ttu-id="8dd1c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd1c-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8dd1c-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dd1c-132">Authorization</span></span> | <span data-ttu-id="8dd1c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8dd1c-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dd1c-135">Content-Type</span></span>  | <span data-ttu-id="8dd1c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dd1c-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dd1c-138">Request body</span></span>

<span data-ttu-id="8dd1c-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8dd1c-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="8dd1c-140">Parameter</span></span>    | <span data-ttu-id="8dd1c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd1c-141">Type</span></span>        | <span data-ttu-id="8dd1c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd1c-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8dd1c-143">ids</span><span class="sxs-lookup"><span data-stu-id="8dd1c-143">ids</span></span>|<span data-ttu-id="8dd1c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8dd1c-144">String collection</span></span>|<span data-ttu-id="8dd1c-145">Коллекция, которая содержит объектные ID групп, роли каталога или roleTemplate ID ролей каталога, в которых необходимо проверить членство.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-145">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="8dd1c-146">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-146">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="8dd1c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd1c-147">Response</span></span>

<span data-ttu-id="8dd1c-148">В случае успешной работы этот метод возвращает код отклика и новый объект `200 OK` коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-148">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dd1c-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dd1c-149">Examples</span></span>

<span data-ttu-id="8dd1c-150">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-150">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8dd1c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dd1c-151">Request</span></span>

<span data-ttu-id="8dd1c-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8dd1c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dd1c-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8dd1c-154">C#</span><span class="sxs-lookup"><span data-stu-id="8dd1c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dd1c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dd1c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dd1c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dd1c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dd1c-157">Java</span><span class="sxs-lookup"><span data-stu-id="8dd1c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8dd1c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd1c-158">Response</span></span>

<span data-ttu-id="8dd1c-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-159">The following is an example of the response.</span></span> 

><span data-ttu-id="8dd1c-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dd1c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

