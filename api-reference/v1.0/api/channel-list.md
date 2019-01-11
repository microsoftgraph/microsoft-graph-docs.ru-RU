---
title: Список каналов
description: Получить список каналов в данной группы.
author: nkramer
localization_priority: Priority
ms.openlocfilehash: e47afbb3b1568a656aff261b015cb5a11403e6e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885507"
---
# <a name="list-channels"></a><span data-ttu-id="865f3-103">Список каналов</span><span class="sxs-lookup"><span data-stu-id="865f3-103">List channels</span></span>



<span data-ttu-id="865f3-104">Получить список [каналов](../resources/channel.md) из этой группы.</span><span class="sxs-lookup"><span data-stu-id="865f3-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="865f3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="865f3-105">Permissions</span></span>
<span data-ttu-id="865f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="865f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="865f3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="865f3-108">Permission type</span></span>      | <span data-ttu-id="865f3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="865f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="865f3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="865f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="865f3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865f3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="865f3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="865f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="865f3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="865f3-113">Not supported.</span></span>    |
|<span data-ttu-id="865f3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="865f3-114">Application</span></span> | <span data-ttu-id="865f3-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865f3-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="865f3-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="865f3-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="865f3-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="865f3-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="865f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="865f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="865f3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="865f3-119">Optional query parameters</span></span>
<span data-ttu-id="865f3-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="865f3-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="865f3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="865f3-121">Request headers</span></span>
| <span data-ttu-id="865f3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="865f3-122">Header</span></span>       | <span data-ttu-id="865f3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="865f3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="865f3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="865f3-124">Authorization</span></span>  | <span data-ttu-id="865f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="865f3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="865f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="865f3-127">Request body</span></span>
<span data-ttu-id="865f3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="865f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="865f3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="865f3-129">Response</span></span>

<span data-ttu-id="865f3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="865f3-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="865f3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="865f3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="865f3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="865f3-132">Request</span></span>
<span data-ttu-id="865f3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="865f3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="865f3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="865f3-134">Response</span></span>
<span data-ttu-id="865f3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="865f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
