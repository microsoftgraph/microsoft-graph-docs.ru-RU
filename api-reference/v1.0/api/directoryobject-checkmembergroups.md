---
title: Проверка групп элементов
description: Проверяет членство в указанном списке групп и возвращает из этого списка эти группы.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ebf38b8f230233b50fa642f7503302afd02b33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555131"
---
# <a name="check-member-groups"></a><span data-ttu-id="cd82f-103">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="cd82f-103">Check member groups</span></span>

<span data-ttu-id="cd82f-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="cd82f-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd82f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd82f-106">Permissions</span></span>
<span data-ttu-id="cd82f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd82f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd82f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd82f-109">Permission type</span></span>      | <span data-ttu-id="cd82f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd82f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd82f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd82f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd82f-112">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd82f-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="cd82f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd82f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd82f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd82f-114">Not supported.</span></span>    |
|<span data-ttu-id="cd82f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd82f-115">Application</span></span> | <span data-ttu-id="cd82f-116">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd82f-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd82f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd82f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="cd82f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd82f-118">Request headers</span></span>
| <span data-ttu-id="cd82f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cd82f-119">Name</span></span>       | <span data-ttu-id="cd82f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cd82f-120">Type</span></span> | <span data-ttu-id="cd82f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cd82f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd82f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd82f-122">Authorization</span></span>  | <span data-ttu-id="cd82f-123">string</span><span class="sxs-lookup"><span data-stu-id="cd82f-123">string</span></span>  | <span data-ttu-id="cd82f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd82f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd82f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd82f-126">Content-Type</span></span>  | <span data-ttu-id="cd82f-127">string</span><span class="sxs-lookup"><span data-stu-id="cd82f-127">string</span></span> | <span data-ttu-id="cd82f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cd82f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd82f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd82f-129">Request body</span></span>
<span data-ttu-id="cd82f-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cd82f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cd82f-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="cd82f-131">Parameter</span></span>    | <span data-ttu-id="cd82f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cd82f-132">Type</span></span>   |<span data-ttu-id="cd82f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cd82f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd82f-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="cd82f-134">groupIds</span></span>|<span data-ttu-id="cd82f-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd82f-135">String collection</span></span>|<span data-ttu-id="cd82f-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="cd82f-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="cd82f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd82f-138">Response</span></span>

<span data-ttu-id="cd82f-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd82f-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd82f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="cd82f-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cd82f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd82f-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="cd82f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd82f-142">Response</span></span>
<span data-ttu-id="cd82f-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd82f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
