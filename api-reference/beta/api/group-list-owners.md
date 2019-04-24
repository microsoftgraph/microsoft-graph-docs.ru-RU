---
title: Список владельцев
description: Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 477a8fd2e647d8bdc3babdcb48bccba469912e93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502088"
---
# <a name="list-owners"></a><span data-ttu-id="40112-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="40112-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40112-p102">Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="40112-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40112-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40112-107">Permissions</span></span>
<span data-ttu-id="40112-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40112-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40112-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40112-110">Permission type</span></span>      | <span data-ttu-id="40112-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40112-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40112-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40112-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40112-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40112-113">Not supported.</span></span>    |
|<span data-ttu-id="40112-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40112-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40112-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40112-115">Not supported.</span></span>    |
|<span data-ttu-id="40112-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40112-116">Application</span></span> | <span data-ttu-id="40112-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40112-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40112-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40112-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40112-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40112-119">Optional query parameters</span></span>
<span data-ttu-id="40112-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="40112-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40112-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40112-121">Request headers</span></span>
| <span data-ttu-id="40112-122">Имя</span><span class="sxs-lookup"><span data-stu-id="40112-122">Name</span></span>       | <span data-ttu-id="40112-123">Тип</span><span class="sxs-lookup"><span data-stu-id="40112-123">Type</span></span> | <span data-ttu-id="40112-124">Описание</span><span class="sxs-lookup"><span data-stu-id="40112-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40112-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="40112-125">Authorization</span></span>  | <span data-ttu-id="40112-126">string</span><span class="sxs-lookup"><span data-stu-id="40112-126">string</span></span>  | <span data-ttu-id="40112-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40112-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40112-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40112-129">Request body</span></span>
<span data-ttu-id="40112-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40112-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40112-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="40112-131">Response</span></span>
<span data-ttu-id="40112-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40112-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40112-133">Пример</span><span class="sxs-lookup"><span data-stu-id="40112-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="40112-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="40112-134">Request</span></span>
<span data-ttu-id="40112-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40112-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="40112-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="40112-136">Response</span></span>
<span data-ttu-id="40112-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40112-137">The following is an example of the response.</span></span>
><span data-ttu-id="40112-138">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="40112-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40112-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40112-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
