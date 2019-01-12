---
title: Проверка групп элементов
description: Проверить членство в заданном списке групп и возвращает из этого списка в эти группы
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ebf38b8f230233b50fa642f7503302afd02b33
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941788"
---
# <a name="check-member-groups"></a><span data-ttu-id="da2d9-103">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="da2d9-103">Check member groups</span></span>

<span data-ttu-id="da2d9-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="da2d9-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="da2d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da2d9-106">Permissions</span></span>
<span data-ttu-id="da2d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da2d9-109">Permission type</span></span>      | <span data-ttu-id="da2d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da2d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da2d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da2d9-112">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da2d9-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="da2d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da2d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2d9-114">Not supported.</span></span>    |
|<span data-ttu-id="da2d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da2d9-115">Application</span></span> | <span data-ttu-id="da2d9-116">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da2d9-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da2d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="da2d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da2d9-118">Request headers</span></span>
| <span data-ttu-id="da2d9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="da2d9-119">Name</span></span>       | <span data-ttu-id="da2d9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="da2d9-120">Type</span></span> | <span data-ttu-id="da2d9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="da2d9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da2d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2d9-122">Authorization</span></span>  | <span data-ttu-id="da2d9-123">string</span><span class="sxs-lookup"><span data-stu-id="da2d9-123">string</span></span>  | <span data-ttu-id="da2d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da2d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da2d9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da2d9-126">Content-Type</span></span>  | <span data-ttu-id="da2d9-127">строка</span><span class="sxs-lookup"><span data-stu-id="da2d9-127">string</span></span> | <span data-ttu-id="da2d9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da2d9-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da2d9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da2d9-129">Request body</span></span>
<span data-ttu-id="da2d9-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="da2d9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da2d9-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="da2d9-131">Parameter</span></span>    | <span data-ttu-id="da2d9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="da2d9-132">Type</span></span>   |<span data-ttu-id="da2d9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="da2d9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da2d9-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="da2d9-134">groupIds</span></span>|<span data-ttu-id="da2d9-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da2d9-135">String collection</span></span>|<span data-ttu-id="da2d9-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="da2d9-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="da2d9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2d9-138">Response</span></span>

<span data-ttu-id="da2d9-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da2d9-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2d9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="da2d9-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da2d9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="da2d9-141">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="da2d9-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2d9-142">Response</span></span>
<span data-ttu-id="da2d9-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da2d9-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
