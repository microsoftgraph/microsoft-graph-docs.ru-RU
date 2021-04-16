---
title: 'servicePrincipal: getMemberObjects'
description: Получение списка групп и ролей каталога, в которых участвует субъект-служба.  Это транзитивная проверка.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d70b5da70b09c6b37c3d1d42040e42cbe4c576f2
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870088"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="527ca-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="527ca-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="527ca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="527ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="527ca-106">Получение списка групп и ролей каталога, в которых участвует [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="527ca-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="527ca-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="527ca-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="527ca-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="527ca-108">Permissions</span></span>
<span data-ttu-id="527ca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="527ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="527ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="527ca-111">Permission type</span></span>      | <span data-ttu-id="527ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="527ca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="527ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="527ca-113">Delegated (work or school account)</span></span> | <span data-ttu-id="527ca-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="527ca-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="527ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="527ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="527ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="527ca-116">Not supported.</span></span>    |
|<span data-ttu-id="527ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="527ca-117">Application</span></span> | <span data-ttu-id="527ca-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527ca-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="527ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="527ca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="527ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="527ca-120">Request headers</span></span>
| <span data-ttu-id="527ca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="527ca-121">Name</span></span>       | <span data-ttu-id="527ca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="527ca-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="527ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="527ca-123">Authorization</span></span> | <span data-ttu-id="527ca-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="527ca-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="527ca-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="527ca-126">Content-type</span></span> | <span data-ttu-id="527ca-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="527ca-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="527ca-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="527ca-129">Request body</span></span>
<span data-ttu-id="527ca-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="527ca-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="527ca-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="527ca-131">Parameter</span></span>    | <span data-ttu-id="527ca-132">Тип</span><span class="sxs-lookup"><span data-stu-id="527ca-132">Type</span></span>   |<span data-ttu-id="527ca-133">Описание</span><span class="sxs-lookup"><span data-stu-id="527ca-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="527ca-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="527ca-134">securityEnabledOnly</span></span>|<span data-ttu-id="527ca-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="527ca-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="527ca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="527ca-136">Response</span></span>

<span data-ttu-id="527ca-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="527ca-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="527ca-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="527ca-138">Examples</span></span>
<span data-ttu-id="527ca-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="527ca-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="527ca-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="527ca-140">Request</span></span>
<span data-ttu-id="527ca-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="527ca-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="527ca-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="527ca-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="527ca-143">C#</span><span class="sxs-lookup"><span data-stu-id="527ca-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="527ca-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="527ca-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="527ca-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="527ca-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="527ca-146">Java</span><span class="sxs-lookup"><span data-stu-id="527ca-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="527ca-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="527ca-147">Response</span></span>
<span data-ttu-id="527ca-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="527ca-148">Here is an example of the response.</span></span> 
><span data-ttu-id="527ca-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="527ca-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



