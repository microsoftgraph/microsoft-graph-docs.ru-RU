---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9d6d149a0e38fb5e02a2c32f9ad218fb95f32911
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565585"
---
# <a name="list-channels"></a><span data-ttu-id="ea4c5-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="ea4c5-103">List channels</span></span>



<span data-ttu-id="ea4c5-104">Получение списка [каналов](../resources/channel.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea4c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea4c5-105">Permissions</span></span>
<span data-ttu-id="ea4c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea4c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea4c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea4c5-108">Permission type</span></span>      | <span data-ttu-id="ea4c5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea4c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea4c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea4c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea4c5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea4c5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea4c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea4c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea4c5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-113">Not supported.</span></span>    |
|<span data-ttu-id="ea4c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea4c5-114">Application</span></span> | <span data-ttu-id="ea4c5-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea4c5-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="ea4c5-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ea4c5-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ea4c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea4c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea4c5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea4c5-119">Optional query parameters</span></span>
<span data-ttu-id="ea4c5-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea4c5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea4c5-121">Request headers</span></span>
| <span data-ttu-id="ea4c5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea4c5-122">Header</span></span>       | <span data-ttu-id="ea4c5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ea4c5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea4c5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea4c5-124">Authorization</span></span>  | <span data-ttu-id="ea4c5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea4c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea4c5-127">Request body</span></span>
<span data-ttu-id="ea4c5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea4c5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea4c5-129">Response</span></span>

<span data-ttu-id="ea4c5-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea4c5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ea4c5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea4c5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea4c5-132">Request</span></span>
<span data-ttu-id="ea4c5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="ea4c5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea4c5-134">Response</span></span>
<span data-ttu-id="ea4c5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea4c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
