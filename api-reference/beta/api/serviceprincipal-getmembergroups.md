---
title: 'servicePrincipal: getMemberGroups'
description: Список групп, в которых участвует субъект-служба.  Это транзитивная проверка.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 66298b90fb794fc4453de5b983b1213a8486cc23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134451"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="ea99d-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ea99d-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="ea99d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea99d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea99d-106">Получение списка групп, участником которых является [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="ea99d-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="ea99d-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ea99d-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea99d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea99d-108">Permissions</span></span>
<span data-ttu-id="ea99d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea99d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea99d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea99d-111">Permission type</span></span>      | <span data-ttu-id="ea99d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea99d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea99d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea99d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea99d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea99d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea99d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea99d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea99d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea99d-116">Not supported.</span></span>    |
|<span data-ttu-id="ea99d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea99d-117">Application</span></span> | <span data-ttu-id="ea99d-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea99d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea99d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea99d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="ea99d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea99d-120">Request headers</span></span>
| <span data-ttu-id="ea99d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ea99d-121">Name</span></span>       | <span data-ttu-id="ea99d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea99d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ea99d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea99d-123">Authorization</span></span> | <span data-ttu-id="ea99d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea99d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea99d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea99d-126">Content-type</span></span> | <span data-ttu-id="ea99d-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea99d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea99d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea99d-129">Request body</span></span>
<span data-ttu-id="ea99d-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ea99d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea99d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ea99d-131">Parameter</span></span>    | <span data-ttu-id="ea99d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ea99d-132">Type</span></span>   |<span data-ttu-id="ea99d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ea99d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea99d-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ea99d-134">securityEnabledOnly</span></span>|<span data-ttu-id="ea99d-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="ea99d-135">Boolean</span></span>|<span data-ttu-id="ea99d-p106">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea99d-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="ea99d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea99d-138">Response</span></span>

<span data-ttu-id="ea99d-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea99d-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea99d-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea99d-140">Examples</span></span>
<span data-ttu-id="ea99d-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ea99d-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ea99d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea99d-142">Request</span></span>
<span data-ttu-id="ea99d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea99d-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea99d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea99d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="ea99d-145">C#</span><span class="sxs-lookup"><span data-stu-id="ea99d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea99d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea99d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea99d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea99d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea99d-148">Java</span><span class="sxs-lookup"><span data-stu-id="ea99d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea99d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea99d-149">Response</span></span>
<span data-ttu-id="ea99d-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea99d-150">Here is an example of the response.</span></span> 
><span data-ttu-id="ea99d-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea99d-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



