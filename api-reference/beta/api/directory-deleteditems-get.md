---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
ms.openlocfilehash: f1db1de878625ffb48357ca6ec58fddea181ef48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074989"
---
# <a name="get-deleted-item"></a><span data-ttu-id="a0abe-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a0abe-103">Get deleted item</span></span>

> <span data-ttu-id="a0abe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0abe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0abe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0abe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0abe-106">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a0abe-106">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a0abe-107">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a0abe-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0abe-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0abe-108">Permissions</span></span>
<span data-ttu-id="a0abe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0abe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="a0abe-111">Для пользователей: User.Read.All, User.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0abe-111">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="a0abe-112">Для групп: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0abe-112">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a0abe-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0abe-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0abe-114">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0abe-114">Optional query parameters</span></span>
<span data-ttu-id="a0abe-115">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0abe-115">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0abe-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0abe-116">Request headers</span></span>
| <span data-ttu-id="a0abe-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a0abe-117">Name</span></span>      |<span data-ttu-id="a0abe-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a0abe-118">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0abe-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0abe-119">Authorization</span></span>  | <span data-ttu-id="a0abe-120">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="a0abe-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a0abe-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a0abe-121">Accept</span></span>  | <span data-ttu-id="a0abe-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a0abe-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0abe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0abe-123">Request body</span></span>
<span data-ttu-id="a0abe-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0abe-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0abe-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0abe-125">Response</span></span>

<span data-ttu-id="a0abe-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0abe-126">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0abe-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a0abe-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0abe-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0abe-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="a0abe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0abe-129">Response</span></span>
<span data-ttu-id="a0abe-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0abe-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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