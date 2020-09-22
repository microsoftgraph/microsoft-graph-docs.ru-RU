---
title: 'Группа: Чеккмемберобжектс'
description: Проверка членства в списке групп или ролей каталогов для указанного объекта Group.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8cb8324c3b812963e461d63807aa2a071ff8a63
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023333"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="324fe-103">Группа: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="324fe-103">group: checkMemberObjects</span></span>

<span data-ttu-id="324fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="324fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="324fe-105">Проверка членства в списке групп или ролей каталогов для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="324fe-105">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="324fe-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="324fe-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="324fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="324fe-107">Permissions</span></span>

<span data-ttu-id="324fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="324fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="324fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="324fe-110">Permission type</span></span>                        | <span data-ttu-id="324fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="324fe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="324fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="324fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="324fe-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="324fe-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="324fe-114">С</span><span class="sxs-lookup"><span data-stu-id="324fe-114">And:</span></span><br><ul><li><span data-ttu-id="324fe-115">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="324fe-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="324fe-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="324fe-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="324fe-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="324fe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="324fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="324fe-118">Not supported.</span></span> |
| <span data-ttu-id="324fe-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="324fe-119">Application</span></span>                            | <span data-ttu-id="324fe-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="324fe-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="324fe-121">С</span><span class="sxs-lookup"><span data-stu-id="324fe-121">And:</span></span><br><ul><li><span data-ttu-id="324fe-122">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="324fe-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="324fe-123">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="324fe-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="324fe-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="324fe-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="324fe-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="324fe-125">Request headers</span></span>

| <span data-ttu-id="324fe-126">Имя</span><span class="sxs-lookup"><span data-stu-id="324fe-126">Name</span></span>          | <span data-ttu-id="324fe-127">Описание</span><span class="sxs-lookup"><span data-stu-id="324fe-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="324fe-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="324fe-128">Authorization</span></span> | <span data-ttu-id="324fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="324fe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="324fe-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="324fe-131">Content-Type</span></span>  | <span data-ttu-id="324fe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="324fe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="324fe-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="324fe-134">Request body</span></span>

<span data-ttu-id="324fe-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="324fe-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="324fe-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="324fe-136">Parameter</span></span>    | <span data-ttu-id="324fe-137">Тип</span><span class="sxs-lookup"><span data-stu-id="324fe-137">Type</span></span>        | <span data-ttu-id="324fe-138">Описание</span><span class="sxs-lookup"><span data-stu-id="324fe-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="324fe-139">ids</span><span class="sxs-lookup"><span data-stu-id="324fe-139">ids</span></span>|<span data-ttu-id="324fe-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="324fe-140">String collection</span></span>| <span data-ttu-id="324fe-141">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="324fe-141">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="324fe-142">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="324fe-142">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="324fe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="324fe-143">Response</span></span>

<span data-ttu-id="324fe-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="324fe-144">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="324fe-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="324fe-145">Examples</span></span>

<span data-ttu-id="324fe-146">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="324fe-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="324fe-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="324fe-147">Request</span></span>

<span data-ttu-id="324fe-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="324fe-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="324fe-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="324fe-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="324fe-150">C#</span><span class="sxs-lookup"><span data-stu-id="324fe-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="324fe-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="324fe-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="324fe-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="324fe-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="324fe-153">Java</span><span class="sxs-lookup"><span data-stu-id="324fe-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="324fe-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="324fe-154">Response</span></span>

<span data-ttu-id="324fe-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="324fe-155">The following is an example of the response.</span></span> 

> <span data-ttu-id="324fe-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="324fe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

