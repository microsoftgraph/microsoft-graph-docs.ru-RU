---
title: 'group: getMemberObjects'
description: 'Возврат всех групп и административных единиц, участником которых является группа. Это транзитивная проверка. Note: группы не могут быть членами ролей каталогов, поэтому роли каталогов не будут возвращены.'
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 73e976ab377ac74d0503e5b94891a6dc616e38fa
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539061"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="010f2-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="010f2-105">group: getMemberObjects</span></span>

<span data-ttu-id="010f2-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="010f2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="010f2-107">Возврат всех групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="010f2-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="010f2-108">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="010f2-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="010f2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="010f2-109">Permissions</span></span>
<span data-ttu-id="010f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="010f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="010f2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="010f2-112">Permission type</span></span>      | <span data-ttu-id="010f2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="010f2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="010f2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="010f2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="010f2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="010f2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="010f2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="010f2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="010f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="010f2-117">Not supported.</span></span>    |
|<span data-ttu-id="010f2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="010f2-118">Application</span></span> | <span data-ttu-id="010f2-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="010f2-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="010f2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="010f2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="010f2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="010f2-121">Request headers</span></span>
| <span data-ttu-id="010f2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="010f2-122">Name</span></span>       | <span data-ttu-id="010f2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="010f2-123">Type</span></span> | <span data-ttu-id="010f2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="010f2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="010f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="010f2-125">Authorization</span></span>  | <span data-ttu-id="010f2-126">string</span><span class="sxs-lookup"><span data-stu-id="010f2-126">string</span></span>  | <span data-ttu-id="010f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="010f2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="010f2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="010f2-129">Request body</span></span>
<span data-ttu-id="010f2-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="010f2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="010f2-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="010f2-131">Parameter</span></span>    | <span data-ttu-id="010f2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="010f2-132">Type</span></span>   |<span data-ttu-id="010f2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="010f2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="010f2-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="010f2-134">securityEnabledOnly</span></span>|<span data-ttu-id="010f2-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="010f2-135">Boolean</span></span>|<span data-ttu-id="010f2-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="010f2-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="010f2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="010f2-138">Response</span></span>
<span data-ttu-id="010f2-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="010f2-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="010f2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="010f2-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="010f2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="010f2-141">Request</span></span>
<span data-ttu-id="010f2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="010f2-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="010f2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="010f2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="010f2-144">C#</span><span class="sxs-lookup"><span data-stu-id="010f2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="010f2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="010f2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="010f2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="010f2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="010f2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="010f2-147">Response</span></span>
<span data-ttu-id="010f2-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="010f2-148">The following is an example of the response.</span></span>
><span data-ttu-id="010f2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="010f2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
