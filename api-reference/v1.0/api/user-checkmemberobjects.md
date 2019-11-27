---
title: 'Пользователь: Чеккмемберобжектс'
description: Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da8993fb65fcc9a0a7bb0f887c3e743b196c686a
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621637"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="f64d6-103">Пользователь: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="f64d6-103">user: checkMemberObjects</span></span>

<span data-ttu-id="f64d6-104">Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="f64d6-104">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="f64d6-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="f64d6-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f64d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f64d6-106">Permissions</span></span>

<span data-ttu-id="f64d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f64d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f64d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f64d6-109">Permission type</span></span>                        | <span data-ttu-id="f64d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f64d6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f64d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f64d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f64d6-112">User. ReadBasic, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="f64d6-113">Дополнительно:</span><span class="sxs-lookup"><span data-stu-id="f64d6-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="f64d6-114">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="f64d6-115">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="f64d6-116">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f64d6-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="f64d6-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f64d6-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="f64d6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f64d6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f64d6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64d6-119">Not supported.</span></span> |
| <span data-ttu-id="f64d6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f64d6-120">Application</span></span>                            | <span data-ttu-id="f64d6-121">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="f64d6-122">С</span><span class="sxs-lookup"><span data-stu-id="f64d6-122">And:</span></span><ul><li><span data-ttu-id="f64d6-123">Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="f64d6-124">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f64d6-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="f64d6-125">Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f64d6-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="f64d6-126">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64d6-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f64d6-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f64d6-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="f64d6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f64d6-128">Request headers</span></span>

| <span data-ttu-id="f64d6-129">Имя</span><span class="sxs-lookup"><span data-stu-id="f64d6-129">Name</span></span>          | <span data-ttu-id="f64d6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f64d6-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f64d6-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f64d6-131">Authorization</span></span> | <span data-ttu-id="f64d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f64d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f64d6-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f64d6-134">Content-Type</span></span>  | <span data-ttu-id="f64d6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f64d6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f64d6-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f64d6-137">Request body</span></span>

<span data-ttu-id="f64d6-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f64d6-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f64d6-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="f64d6-139">Parameter</span></span>    | <span data-ttu-id="f64d6-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f64d6-140">Type</span></span>        | <span data-ttu-id="f64d6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f64d6-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f64d6-142">ids</span><span class="sxs-lookup"><span data-stu-id="f64d6-142">ids</span></span>|<span data-ttu-id="f64d6-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f64d6-143">String collection</span></span>|<span data-ttu-id="f64d6-144">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="f64d6-144">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="f64d6-145">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="f64d6-145">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="f64d6-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f64d6-146">Response</span></span>

<span data-ttu-id="f64d6-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f64d6-147">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f64d6-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="f64d6-148">Examples</span></span>

<span data-ttu-id="f64d6-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f64d6-149">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f64d6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f64d6-150">Request</span></span>

<span data-ttu-id="f64d6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f64d6-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f64d6-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f64d6-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f64d6-153">C#</span><span class="sxs-lookup"><span data-stu-id="f64d6-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f64d6-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f64d6-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f64d6-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f64d6-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f64d6-156">Java</span><span class="sxs-lookup"><span data-stu-id="f64d6-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f64d6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f64d6-157">Response</span></span>

<span data-ttu-id="f64d6-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f64d6-158">The following is an example of the response.</span></span> 

><span data-ttu-id="f64d6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f64d6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
