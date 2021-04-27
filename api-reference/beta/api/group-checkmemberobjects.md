---
title: 'группа: checkMemberObjects'
description: Проверьте членство в списке групп, ролей каталогов или административных единиц для указанного объекта группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4c5b158faa3152db0143334e4f17fb631b920ecb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042074"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="55613-103">группа: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="55613-103">group: checkMemberObjects</span></span>

<span data-ttu-id="55613-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55613-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55613-105">Проверка членства в списке групп или административных подразделений для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="55613-105">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="55613-106">Этот метод является транзитным.</span><span class="sxs-lookup"><span data-stu-id="55613-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="55613-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55613-107">Permissions</span></span>

<span data-ttu-id="55613-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55613-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55613-110">Permission type</span></span>                        | <span data-ttu-id="55613-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55613-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55613-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55613-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="55613-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55613-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="55613-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55613-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55613-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55613-115">Not supported.</span></span> |
| <span data-ttu-id="55613-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55613-116">Application</span></span>                            | <span data-ttu-id="55613-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55613-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55613-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55613-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="55613-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55613-119">Request headers</span></span>

| <span data-ttu-id="55613-120">Имя</span><span class="sxs-lookup"><span data-stu-id="55613-120">Name</span></span>          | <span data-ttu-id="55613-121">Описание</span><span class="sxs-lookup"><span data-stu-id="55613-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55613-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55613-122">Authorization</span></span> | <span data-ttu-id="55613-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="55613-123">Bearer {token}</span></span> |
| <span data-ttu-id="55613-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55613-124">Content-Type</span></span>  | <span data-ttu-id="55613-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55613-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55613-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55613-126">Request body</span></span>

<span data-ttu-id="55613-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55613-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55613-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="55613-128">Parameter</span></span>    | <span data-ttu-id="55613-129">Тип</span><span class="sxs-lookup"><span data-stu-id="55613-129">Type</span></span>        | <span data-ttu-id="55613-130">Описание</span><span class="sxs-lookup"><span data-stu-id="55613-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55613-131">ids</span><span class="sxs-lookup"><span data-stu-id="55613-131">ids</span></span>|<span data-ttu-id="55613-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55613-132">String collection</span></span>| <span data-ttu-id="55613-133">Коллекция, в которой содержатся объектные ИД групп, роли каталога, административные единицы или roleTemplate ID ролей каталога, в которых необходимо проверить членство.</span><span class="sxs-lookup"><span data-stu-id="55613-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="55613-134">Может быть указано до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="55613-134">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="55613-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="55613-135">Response</span></span>

<span data-ttu-id="55613-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55613-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55613-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="55613-137">Examples</span></span>

<span data-ttu-id="55613-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="55613-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="55613-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="55613-139">Request</span></span>

<span data-ttu-id="55613-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55613-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55613-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="55613-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="55613-142">C#</span><span class="sxs-lookup"><span data-stu-id="55613-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55613-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55613-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55613-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55613-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55613-145">Java</span><span class="sxs-lookup"><span data-stu-id="55613-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55613-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="55613-146">Response</span></span>

<span data-ttu-id="55613-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55613-147">The following is an example of the response.</span></span> 

> <span data-ttu-id="55613-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55613-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


