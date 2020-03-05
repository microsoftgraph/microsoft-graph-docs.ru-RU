---
title: 'Группа: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта Group.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 736c46ab52d9f8aff3ba014f5bcfae60f0d2ce09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420586"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="e8a68-103">Группа: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="e8a68-103">group: checkMemberObjects</span></span>

<span data-ttu-id="e8a68-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e8a68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a68-105">Проверка членства в списке групп или административных единиц для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="e8a68-105">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="e8a68-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="e8a68-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a68-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a68-107">Permissions</span></span>

<span data-ttu-id="e8a68-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8a68-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a68-110">Permission type</span></span>                        | <span data-ttu-id="e8a68-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8a68-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8a68-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8a68-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8a68-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a68-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="e8a68-114">С</span><span class="sxs-lookup"><span data-stu-id="e8a68-114">And:</span></span><br><ul><li><span data-ttu-id="e8a68-115">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8a68-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="e8a68-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8a68-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e8a68-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8a68-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a68-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a68-118">Not supported.</span></span> |
| <span data-ttu-id="e8a68-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8a68-119">Application</span></span>                            | <span data-ttu-id="e8a68-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a68-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="e8a68-121">С</span><span class="sxs-lookup"><span data-stu-id="e8a68-121">And:</span></span><br><ul><li><span data-ttu-id="e8a68-122">При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8a68-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="e8a68-123">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a68-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a68-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8a68-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="e8a68-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8a68-125">Request headers</span></span>

| <span data-ttu-id="e8a68-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e8a68-126">Name</span></span>          | <span data-ttu-id="e8a68-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a68-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e8a68-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a68-128">Authorization</span></span> | <span data-ttu-id="e8a68-129">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e8a68-129">Bearer {token}</span></span> |
| <span data-ttu-id="e8a68-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8a68-130">Content-Type</span></span>  | <span data-ttu-id="e8a68-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e8a68-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8a68-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8a68-132">Request body</span></span>

<span data-ttu-id="e8a68-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e8a68-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8a68-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="e8a68-134">Parameter</span></span>    | <span data-ttu-id="e8a68-135">Тип</span><span class="sxs-lookup"><span data-stu-id="e8a68-135">Type</span></span>        | <span data-ttu-id="e8a68-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a68-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8a68-137">ids</span><span class="sxs-lookup"><span data-stu-id="e8a68-137">ids</span></span>|<span data-ttu-id="e8a68-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8a68-138">String collection</span></span>| <span data-ttu-id="e8a68-139">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="e8a68-139">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="e8a68-140">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="e8a68-140">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="e8a68-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a68-141">Response</span></span>

<span data-ttu-id="e8a68-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8a68-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8a68-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8a68-143">Examples</span></span>

<span data-ttu-id="e8a68-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e8a68-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e8a68-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8a68-145">Request</span></span>

<span data-ttu-id="e8a68-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8a68-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8a68-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a68-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="e8a68-148">C#</span><span class="sxs-lookup"><span data-stu-id="e8a68-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8a68-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8a68-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8a68-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8a68-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8a68-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a68-151">Response</span></span>

<span data-ttu-id="e8a68-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8a68-152">The following is an example of the response.</span></span> 

> <span data-ttu-id="e8a68-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8a68-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
