---
title: ПереЧисление пользователя memberOf
description: Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь. Эта операция не является транзитивной.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a9b8b111a55a76390ef0a2434ffd19d56423b80
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334866"
---
# <a name="list-user-memberof"></a><span data-ttu-id="19faa-104">ПереЧисление пользователя memberOf</span><span class="sxs-lookup"><span data-stu-id="19faa-104">List user memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19faa-105">Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="19faa-105">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="19faa-106">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="19faa-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="19faa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19faa-107">Permissions</span></span>

<span data-ttu-id="19faa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19faa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19faa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19faa-110">Permission type</span></span>      | <span data-ttu-id="19faa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19faa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19faa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19faa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19faa-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19faa-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19faa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19faa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19faa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19faa-115">Not supported.</span></span>    |
|<span data-ttu-id="19faa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19faa-116">Application</span></span> | <span data-ttu-id="19faa-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19faa-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19faa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19faa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19faa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19faa-119">Optional query parameters</span></span>

<span data-ttu-id="19faa-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19faa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19faa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19faa-121">Request headers</span></span>
| <span data-ttu-id="19faa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19faa-122">Header</span></span>       | <span data-ttu-id="19faa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="19faa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19faa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19faa-124">Authorization</span></span>  | <span data-ttu-id="19faa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19faa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19faa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="19faa-127">Accept</span></span>  | <span data-ttu-id="19faa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="19faa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19faa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19faa-129">Request body</span></span>

<span data-ttu-id="19faa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19faa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19faa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="19faa-131">Response</span></span>

<span data-ttu-id="19faa-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19faa-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19faa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="19faa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="19faa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="19faa-134">Request</span></span>

<span data-ttu-id="19faa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19faa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/me/memberOf
```

### <a name="response"></a><span data-ttu-id="19faa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="19faa-136">Response</span></span>

<span data-ttu-id="19faa-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19faa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
