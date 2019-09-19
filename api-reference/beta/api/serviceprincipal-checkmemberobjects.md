---
title: 'servicePrincipal: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 512582a8f8413867aeff0ce168c5b5748ed38fc7
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041868"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="151b3-103">servicePrincipal: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="151b3-103">servicePrincipal: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="151b3-104">Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта участника службы.</span><span class="sxs-lookup"><span data-stu-id="151b3-104">Check for membership in a list of groups, directory roles, or administrative units for the specified service principle object.</span></span> <span data-ttu-id="151b3-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="151b3-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="151b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="151b3-106">Permissions</span></span>

<span data-ttu-id="151b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="151b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="151b3-109">Permission type</span></span>                        | <span data-ttu-id="151b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="151b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="151b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="151b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="151b3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="151b3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="151b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="151b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="151b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="151b3-114">Not supported.</span></span> |
| <span data-ttu-id="151b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="151b3-115">Application</span></span>                            | <span data-ttu-id="151b3-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="151b3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="151b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="151b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="151b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="151b3-118">Request headers</span></span>

| <span data-ttu-id="151b3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="151b3-119">Name</span></span>          | <span data-ttu-id="151b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="151b3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="151b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="151b3-121">Authorization</span></span> | <span data-ttu-id="151b3-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="151b3-122">Bearer {token}</span></span> |
| <span data-ttu-id="151b3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="151b3-123">Content-Type</span></span>  | <span data-ttu-id="151b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="151b3-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="151b3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="151b3-125">Request body</span></span>

<span data-ttu-id="151b3-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="151b3-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="151b3-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="151b3-127">Parameter</span></span>    | <span data-ttu-id="151b3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="151b3-128">Type</span></span>        | <span data-ttu-id="151b3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="151b3-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="151b3-130">ids</span><span class="sxs-lookup"><span data-stu-id="151b3-130">ids</span></span>|<span data-ttu-id="151b3-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="151b3-131">String collection</span></span>|<span data-ttu-id="151b3-132">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="151b3-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="151b3-133">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="151b3-133">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="151b3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="151b3-134">Response</span></span>

<span data-ttu-id="151b3-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="151b3-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="151b3-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="151b3-136">Examples</span></span>

<span data-ttu-id="151b3-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="151b3-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="151b3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="151b3-138">Request</span></span>

<span data-ttu-id="151b3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="151b3-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="151b3-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="151b3-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="151b3-141">C#</span><span class="sxs-lookup"><span data-stu-id="151b3-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="151b3-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="151b3-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="151b3-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="151b3-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="151b3-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="151b3-144">Response</span></span>

<span data-ttu-id="151b3-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="151b3-145">The following is an example of the response.</span></span> 

> <span data-ttu-id="151b3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="151b3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
