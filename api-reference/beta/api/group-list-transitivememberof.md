---
title: Доверия транзитивных член группы списка
description: Получите административные единиц измерения, которые должна быть членом группы и группы.  Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы. В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.
ms.openlocfilehash: e622ee484a4070560c38528bccfe7f12e2172d54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077282"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="42912-105">Доверия транзитивных член группы списка</span><span class="sxs-lookup"><span data-stu-id="42912-105">List group transitive memberOf</span></span>

> <span data-ttu-id="42912-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42912-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42912-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42912-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42912-108">Получите административные единиц измерения, которые должна быть членом группы и группы.</span><span class="sxs-lookup"><span data-stu-id="42912-108">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="42912-109">Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы.</span><span class="sxs-lookup"><span data-stu-id="42912-109">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="42912-110">В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="42912-110">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="42912-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42912-111">Permissions</span></span>

<span data-ttu-id="42912-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42912-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42912-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42912-114">Permission type</span></span>      | <span data-ttu-id="42912-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42912-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42912-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42912-116">Delegated (work or school account)</span></span> | <span data-ttu-id="42912-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42912-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42912-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42912-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42912-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42912-119">Not supported.</span></span>    |
|<span data-ttu-id="42912-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42912-120">Application</span></span> | <span data-ttu-id="42912-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42912-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42912-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42912-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42912-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42912-123">Optional query parameters</span></span>
<span data-ttu-id="42912-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42912-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42912-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42912-125">Request headers</span></span>
| <span data-ttu-id="42912-126">Имя</span><span class="sxs-lookup"><span data-stu-id="42912-126">Name</span></span>       | <span data-ttu-id="42912-127">Тип</span><span class="sxs-lookup"><span data-stu-id="42912-127">Type</span></span> | <span data-ttu-id="42912-128">Описание</span><span class="sxs-lookup"><span data-stu-id="42912-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42912-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="42912-129">Authorization</span></span>  | <span data-ttu-id="42912-130">string</span><span class="sxs-lookup"><span data-stu-id="42912-130">string</span></span>  | <span data-ttu-id="42912-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42912-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42912-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42912-133">Request body</span></span>
<span data-ttu-id="42912-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42912-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42912-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="42912-135">Response</span></span>
<span data-ttu-id="42912-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42912-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42912-137">Пример</span><span class="sxs-lookup"><span data-stu-id="42912-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="42912-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="42912-138">Request</span></span>
<span data-ttu-id="42912-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42912-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="42912-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="42912-140">Response</span></span>

<span data-ttu-id="42912-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42912-141">The following is an example of the response.</span></span>
><span data-ttu-id="42912-142">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="42912-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42912-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42912-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->