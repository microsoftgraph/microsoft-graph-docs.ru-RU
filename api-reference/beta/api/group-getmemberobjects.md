---
title: 'group: getMemberObjects'
description: 'Возврат всех групп и административных единиц, участником которых является группа. Это транзитивная проверка. Note: группы не могут быть членами ролей каталогов, поэтому роли каталогов не будут возвращены.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0bfa66ae32eb8f47c840d7d58d69103edbf35241
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329777"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="c5879-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c5879-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5879-106">Возврат всех групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="c5879-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="c5879-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="c5879-107">The check is transitive.</span></span> <span data-ttu-id="c5879-108">Note: группы не могут быть членами ролей каталогов, поэтому роли каталогов не будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="c5879-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5879-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5879-109">Permissions</span></span>
<span data-ttu-id="c5879-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5879-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5879-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5879-112">Permission type</span></span>      | <span data-ttu-id="c5879-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5879-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5879-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5879-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c5879-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5879-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5879-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5879-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5879-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5879-117">Not supported.</span></span>    |
|<span data-ttu-id="c5879-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5879-118">Application</span></span> | <span data-ttu-id="c5879-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5879-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5879-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5879-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="c5879-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5879-121">Request headers</span></span>
| <span data-ttu-id="c5879-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c5879-122">Name</span></span>       | <span data-ttu-id="c5879-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c5879-123">Type</span></span> | <span data-ttu-id="c5879-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c5879-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5879-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5879-125">Authorization</span></span>  | <span data-ttu-id="c5879-126">string</span><span class="sxs-lookup"><span data-stu-id="c5879-126">string</span></span>  | <span data-ttu-id="c5879-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5879-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5879-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5879-129">Request body</span></span>
<span data-ttu-id="c5879-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5879-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5879-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5879-131">Parameter</span></span>    | <span data-ttu-id="c5879-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c5879-132">Type</span></span>   |<span data-ttu-id="c5879-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c5879-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5879-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c5879-134">securityEnabledOnly</span></span>|<span data-ttu-id="c5879-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="c5879-135">Boolean</span></span>|<span data-ttu-id="c5879-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c5879-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="c5879-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5879-138">Response</span></span>
<span data-ttu-id="c5879-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="c5879-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="c5879-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c5879-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c5879-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5879-141">Request</span></span>
<span data-ttu-id="c5879-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5879-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="c5879-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5879-143">Response</span></span>
<span data-ttu-id="c5879-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5879-144">The following is an example of the response.</span></span>
><span data-ttu-id="c5879-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5879-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
