---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 905b65c5d02bd27ffad17f30290c5ea36118bff3
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108917"
---
# <a name="list-deleted-items"></a><span data-ttu-id="a5712-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="a5712-103">List deleted items</span></span>

<span data-ttu-id="a5712-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5712-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5712-105">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a5712-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a5712-106">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](../resources/application.md) [групповых и](../resources/group.md) [пользовательских](../resources/user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5712-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5712-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5712-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="a5712-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="a5712-110">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="a5712-110">For applications:</span></span>

|<span data-ttu-id="a5712-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5712-111">Permission type</span></span>      | <span data-ttu-id="a5712-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5712-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5712-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5712-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5712-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5712-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5712-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5712-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5712-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5712-116">Not supported.</span></span>    |
|<span data-ttu-id="a5712-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5712-117">Application</span></span> | <span data-ttu-id="a5712-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5712-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="a5712-119">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="a5712-119">For users:</span></span>

|<span data-ttu-id="a5712-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5712-120">Permission type</span></span>      | <span data-ttu-id="a5712-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5712-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5712-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5712-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a5712-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5712-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a5712-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5712-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5712-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5712-125">Not supported.</span></span> |
|<span data-ttu-id="a5712-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5712-126">Application</span></span> | <span data-ttu-id="a5712-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5712-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="a5712-128">Для групп:</span><span class="sxs-lookup"><span data-stu-id="a5712-128">For groups:</span></span>

|<span data-ttu-id="a5712-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5712-129">Permission type</span></span>      | <span data-ttu-id="a5712-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5712-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5712-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5712-131">Delegated (work or school account)</span></span> | <span data-ttu-id="a5712-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5712-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a5712-133">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5712-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5712-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5712-134">Not supported.</span></span>    |
|<span data-ttu-id="a5712-135">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5712-135">Application</span></span> | <span data-ttu-id="a5712-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5712-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5712-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5712-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
GET /directory/deletedItems/microsoft.graph.device
```

<span data-ttu-id="a5712-138">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="a5712-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="a5712-139">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="a5712-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="a5712-140">Вызов GET/directory/deletedItems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5712-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a5712-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5712-141">Optional query parameters</span></span>
<span data-ttu-id="a5712-142">Этот метод поддерживает параметр `$orderBy` [запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5712-142">This method supports the `$orderBy` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span> 

### <a name="examples-using-the-orderby-odata-query-parameter"></a><span data-ttu-id="a5712-143">Примеры использования параметра запроса $orderBy OData</span><span class="sxs-lookup"><span data-stu-id="a5712-143">Examples using the $orderBy OData query parameter</span></span>

<span data-ttu-id="a5712-144">Параметр запроса OData поддерживается в удаленных свойствах `$orderBy` **объектовDateTime,** **displayName** и **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="a5712-144">The `$orderBy` OData query parameter is supported on the **deletedDateTime**, **displayName**, and **userPrincipalName** properties of the deleted object types.</span></span> <span data-ttu-id="a5712-145">В **свойстве deletedDateTime** запрос требует [](/graph/aad-advanced-queries) добавления расширенных параметров запроса (заглавная строка **ConsistencyLevel** и `true` `$count=true` строка запросов).</span><span class="sxs-lookup"><span data-stu-id="a5712-145">On the **deletedDateTime** property, the query requires adding the [advanced query parameters](/graph/aad-advanced-queries) (**ConsistencyLevel** header set to `true` and `$count=true` query string).</span></span>

| <span data-ttu-id="a5712-146">Литой OData</span><span class="sxs-lookup"><span data-stu-id="a5712-146">OData cast</span></span> | <span data-ttu-id="a5712-147">Свойства, поддерживающие $orderBy</span><span class="sxs-lookup"><span data-stu-id="a5712-147">Properties supporting $orderBy</span></span> | <span data-ttu-id="a5712-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a5712-148">Example</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="a5712-149">microsoft.graph.user</span><span class="sxs-lookup"><span data-stu-id="a5712-149">microsoft.graph.user</span></span> | <span data-ttu-id="a5712-150">deletedDateTime, displayName, userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a5712-150">deletedDateTime, displayName, userPrincipalName</span></span> | <span data-ttu-id="a5712-151">/directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a5712-151">/directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName</span></span> |
| <span data-ttu-id="a5712-152">microsoft.graph.group</span><span class="sxs-lookup"><span data-stu-id="a5712-152">microsoft.graph.group</span></span> | <span data-ttu-id="a5712-153">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="a5712-153">deletedDateTime, displayName</span></span> | <span data-ttu-id="a5712-154">/directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true</span><span class="sxs-lookup"><span data-stu-id="a5712-154">/directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true</span></span> |
| <span data-ttu-id="a5712-155">microsoft.graph.application</span><span class="sxs-lookup"><span data-stu-id="a5712-155">microsoft.graph.application</span></span> | <span data-ttu-id="a5712-156">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="a5712-156">deletedDateTime, displayName</span></span> | <span data-ttu-id="a5712-157">/directory/deletedItems/microsoft.graph.application?$orderBy=displayName</span><span class="sxs-lookup"><span data-stu-id="a5712-157">/directory/deletedItems/microsoft.graph.application?$orderBy=displayName</span></span> |
| <span data-ttu-id="a5712-158">microsoft.graph.device</span><span class="sxs-lookup"><span data-stu-id="a5712-158">microsoft.graph.device</span></span> | <span data-ttu-id="a5712-159">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="a5712-159">deletedDateTime, displayName</span></span> | <span data-ttu-id="a5712-160">/directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true</span><span class="sxs-lookup"><span data-stu-id="a5712-160">/directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a5712-161">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5712-161">Request headers</span></span>
| <span data-ttu-id="a5712-162">Имя</span><span class="sxs-lookup"><span data-stu-id="a5712-162">Name</span></span>      |<span data-ttu-id="a5712-163">Описание</span><span class="sxs-lookup"><span data-stu-id="a5712-163">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5712-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5712-164">Authorization</span></span>  | <span data-ttu-id="a5712-165">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="a5712-165">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a5712-166">Accept</span><span class="sxs-lookup"><span data-stu-id="a5712-166">Accept</span></span>  | <span data-ttu-id="a5712-167">application/json</span><span class="sxs-lookup"><span data-stu-id="a5712-167">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5712-168">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5712-168">Request body</span></span>
<span data-ttu-id="a5712-169">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5712-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5712-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5712-170">Response</span></span>

<span data-ttu-id="a5712-171">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5712-171">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5712-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a5712-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5712-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5712-173">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```

### <a name="response"></a><span data-ttu-id="a5712-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5712-174">Response</span></span>
<span data-ttu-id="a5712-175">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5712-175">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
