---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: lleonard-msft
ms.openlocfilehash: e3a42fffba9a447661010ac9f6f5cff19df880c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353713"
---
# <a name="get-deleted-item"></a><span data-ttu-id="adc01-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="adc01-103">Get deleted item</span></span>

<span data-ttu-id="adc01-104">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="adc01-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="adc01-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="adc01-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="adc01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adc01-106">Permissions</span></span>
<span data-ttu-id="adc01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adc01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="adc01-109">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="adc01-109">For users:</span></span>

|<span data-ttu-id="adc01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adc01-110">Permission type</span></span>      | <span data-ttu-id="adc01-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adc01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adc01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adc01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="adc01-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adc01-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="adc01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adc01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adc01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adc01-115">Not supported.</span></span> |
|<span data-ttu-id="adc01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adc01-116">Application</span></span> | <span data-ttu-id="adc01-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adc01-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="adc01-118">Для групп:</span><span class="sxs-lookup"><span data-stu-id="adc01-118">For groups:</span></span>

|<span data-ttu-id="adc01-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adc01-119">Permission type</span></span>      | <span data-ttu-id="adc01-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adc01-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adc01-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adc01-121">Delegated (work or school account)</span></span> | <span data-ttu-id="adc01-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adc01-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="adc01-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adc01-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adc01-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adc01-124">Not supported.</span></span>    |
|<span data-ttu-id="adc01-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adc01-125">Application</span></span> | <span data-ttu-id="adc01-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adc01-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adc01-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adc01-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adc01-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="adc01-128">Optional query parameters</span></span>
<span data-ttu-id="adc01-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="adc01-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adc01-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adc01-130">Request headers</span></span>
| <span data-ttu-id="adc01-131">Имя</span><span class="sxs-lookup"><span data-stu-id="adc01-131">Name</span></span>      |<span data-ttu-id="adc01-132">Описание</span><span class="sxs-lookup"><span data-stu-id="adc01-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="adc01-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="adc01-133">Authorization</span></span>  | <span data-ttu-id="adc01-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="adc01-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="adc01-135">Accept</span><span class="sxs-lookup"><span data-stu-id="adc01-135">Accept</span></span>  | <span data-ttu-id="adc01-136">application/json</span><span class="sxs-lookup"><span data-stu-id="adc01-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="adc01-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adc01-137">Request body</span></span>
<span data-ttu-id="adc01-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adc01-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adc01-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="adc01-139">Response</span></span>

<span data-ttu-id="adc01-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adc01-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="adc01-141">Пример</span><span class="sxs-lookup"><span data-stu-id="adc01-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adc01-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="adc01-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="adc01-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="adc01-143">Response</span></span>
<span data-ttu-id="adc01-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adc01-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->