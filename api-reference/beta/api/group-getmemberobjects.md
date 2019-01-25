---
title: 'group: getMemberObjects'
description: 'Возвращение всех групп и административных единиц, в которых состоит группа. Проверка доверия транзитивных. Примечание: Группы не может быть члены роли каталога, поэтому роли не каталог не возвращается.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4b71a683d3c311acc36ca0ab669c5d6d44180f31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518718"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="8a320-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8a320-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a320-106">Возвращение всех групп и административных единиц, в которых состоит группа.</span><span class="sxs-lookup"><span data-stu-id="8a320-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="8a320-107">Проверка доверия транзитивных.</span><span class="sxs-lookup"><span data-stu-id="8a320-107">The check is transitive.</span></span> <span data-ttu-id="8a320-108">Примечание: Группы не может быть члены роли каталога, поэтому роли не каталог не возвращается.</span><span class="sxs-lookup"><span data-stu-id="8a320-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a320-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a320-109">Permissions</span></span>
<span data-ttu-id="8a320-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a320-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a320-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a320-112">Permission type</span></span>      | <span data-ttu-id="8a320-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a320-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a320-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a320-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8a320-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a320-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a320-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a320-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a320-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a320-117">Not supported.</span></span>    |
|<span data-ttu-id="8a320-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a320-118">Application</span></span> | <span data-ttu-id="8a320-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a320-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a320-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a320-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="8a320-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a320-121">Request headers</span></span>
| <span data-ttu-id="8a320-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8a320-122">Name</span></span>       | <span data-ttu-id="8a320-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8a320-123">Type</span></span> | <span data-ttu-id="8a320-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8a320-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a320-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a320-125">Authorization</span></span>  | <span data-ttu-id="8a320-126">string</span><span class="sxs-lookup"><span data-stu-id="8a320-126">string</span></span>  | <span data-ttu-id="8a320-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a320-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a320-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a320-129">Request body</span></span>
<span data-ttu-id="8a320-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8a320-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a320-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="8a320-131">Parameter</span></span>    | <span data-ttu-id="8a320-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8a320-132">Type</span></span>   |<span data-ttu-id="8a320-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8a320-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a320-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="8a320-134">securityEnabledOnly</span></span>|<span data-ttu-id="8a320-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="8a320-135">Boolean</span></span>|<span data-ttu-id="8a320-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8a320-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="8a320-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a320-138">Response</span></span>
<span data-ttu-id="8a320-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="8a320-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="8a320-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8a320-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8a320-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a320-141">Request</span></span>
<span data-ttu-id="8a320-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a320-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8a320-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a320-143">Response</span></span>
<span data-ttu-id="8a320-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a320-144">The following is an example of the response.</span></span>
><span data-ttu-id="8a320-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a320-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
