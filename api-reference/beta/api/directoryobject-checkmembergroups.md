---
title: Проверка групп элементов
description: Проверить членство в заданном списке групп и возвращает из этого списка в эти группы
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93ff0a0cb215e489490e50bde40f56e5b562be95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971090"
---
# <a name="check-member-groups"></a><span data-ttu-id="4fa3b-103">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="4fa3b-103">Check member groups</span></span>

> <span data-ttu-id="4fa3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fa3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4fa3b-106">Проверьте членство в заданном списке групп и возвращает из этого списка в эти группы, которые указанного пользователя, группы, участника службы или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="4fa3b-107">Эта функция транзитивное.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fa3b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa3b-108">Permissions</span></span>
<span data-ttu-id="4fa3b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fa3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4fa3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa3b-111">Permission type</span></span>      | <span data-ttu-id="4fa3b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fa3b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fa3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fa3b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4fa3b-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fa3b-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="4fa3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fa3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fa3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-116">Not supported.</span></span>    |
|<span data-ttu-id="4fa3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fa3b-117">Application</span></span> | <span data-ttu-id="4fa3b-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fa3b-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fa3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fa3b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="4fa3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fa3b-120">Request headers</span></span>
| <span data-ttu-id="4fa3b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4fa3b-121">Name</span></span>       | <span data-ttu-id="4fa3b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4fa3b-122">Type</span></span> | <span data-ttu-id="4fa3b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4fa3b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4fa3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fa3b-124">Authorization</span></span>  | <span data-ttu-id="4fa3b-125">строка</span><span class="sxs-lookup"><span data-stu-id="4fa3b-125">string</span></span>  | <span data-ttu-id="4fa3b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fa3b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4fa3b-128">Content-Type</span></span>  | <span data-ttu-id="4fa3b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4fa3b-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fa3b-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fa3b-130">Request body</span></span>
<span data-ttu-id="4fa3b-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4fa3b-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="4fa3b-132">Parameter</span></span>    | <span data-ttu-id="4fa3b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4fa3b-133">Type</span></span>   |<span data-ttu-id="4fa3b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4fa3b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fa3b-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="4fa3b-135">groupIds</span></span>|<span data-ttu-id="4fa3b-136">String</span><span class="sxs-lookup"><span data-stu-id="4fa3b-136">String</span></span>|<span data-ttu-id="4fa3b-p105">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="4fa3b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fa3b-139">Response</span></span>

<span data-ttu-id="4fa3b-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fa3b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4fa3b-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4fa3b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fa3b-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="4fa3b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fa3b-143">Response</span></span>
<span data-ttu-id="4fa3b-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fa3b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
