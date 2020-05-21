---
title: 'servicePrincipal: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c70bc51af3a26d00b48ccf97302c9754fff9efd6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334097"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="01367-103">servicePrincipal: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="01367-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="01367-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01367-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01367-105">Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="01367-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="01367-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="01367-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="01367-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01367-107">Permissions</span></span>

<span data-ttu-id="01367-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01367-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01367-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01367-110">Permission type</span></span>                        | <span data-ttu-id="01367-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01367-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01367-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01367-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01367-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01367-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="01367-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01367-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01367-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01367-115">Not supported.</span></span> |
| <span data-ttu-id="01367-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01367-116">Application</span></span>                            | <span data-ttu-id="01367-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01367-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01367-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01367-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="01367-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01367-119">Request headers</span></span>

| <span data-ttu-id="01367-120">Имя</span><span class="sxs-lookup"><span data-stu-id="01367-120">Name</span></span>          | <span data-ttu-id="01367-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01367-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="01367-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01367-122">Authorization</span></span> | <span data-ttu-id="01367-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="01367-123">Bearer {token}</span></span> |
| <span data-ttu-id="01367-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01367-124">Content-Type</span></span>  | <span data-ttu-id="01367-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01367-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01367-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01367-126">Request body</span></span>

<span data-ttu-id="01367-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="01367-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01367-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="01367-128">Parameter</span></span>    | <span data-ttu-id="01367-129">Тип</span><span class="sxs-lookup"><span data-stu-id="01367-129">Type</span></span>        | <span data-ttu-id="01367-130">Описание</span><span class="sxs-lookup"><span data-stu-id="01367-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01367-131">ids</span><span class="sxs-lookup"><span data-stu-id="01367-131">ids</span></span>|<span data-ttu-id="01367-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="01367-132">String collection</span></span>|<span data-ttu-id="01367-133">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="01367-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="01367-134">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="01367-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="01367-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01367-135">Response</span></span>

<span data-ttu-id="01367-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01367-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01367-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="01367-137">Examples</span></span>

<span data-ttu-id="01367-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="01367-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="01367-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="01367-139">Request</span></span>

<span data-ttu-id="01367-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01367-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="01367-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="01367-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="01367-142">C#</span><span class="sxs-lookup"><span data-stu-id="01367-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01367-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01367-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01367-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01367-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01367-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="01367-145">Response</span></span>

<span data-ttu-id="01367-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01367-146">The following is an example of the response.</span></span> 

> <span data-ttu-id="01367-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01367-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
