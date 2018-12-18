---
title: Список каналов
description: Получить список каналов в данной группы.
author: nkramer
ms.openlocfilehash: 4a43c1abe07ce3c2e6c0f56c83151e5601f2824c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309354"
---
# <a name="list-channels"></a><span data-ttu-id="07425-103">Список каналов</span><span class="sxs-lookup"><span data-stu-id="07425-103">List channels</span></span>

> <span data-ttu-id="07425-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07425-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07425-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07425-106">Получить список [каналов](../resources/channel.md) из этой группы.</span><span class="sxs-lookup"><span data-stu-id="07425-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="07425-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07425-107">Permissions</span></span>
<span data-ttu-id="07425-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="07425-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07425-110">Permission type</span></span>      | <span data-ttu-id="07425-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07425-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07425-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07425-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07425-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07425-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07425-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07425-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07425-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07425-115">Not supported.</span></span>    |
|<span data-ttu-id="07425-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07425-116">Application</span></span> | <span data-ttu-id="07425-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07425-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="07425-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="07425-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="07425-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="07425-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="07425-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07425-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07425-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07425-121">Optional query parameters</span></span>
<span data-ttu-id="07425-122">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07425-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07425-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07425-123">Request headers</span></span>
| <span data-ttu-id="07425-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07425-124">Header</span></span>       | <span data-ttu-id="07425-125">Значение</span><span class="sxs-lookup"><span data-stu-id="07425-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07425-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07425-126">Authorization</span></span>  | <span data-ttu-id="07425-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07425-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07425-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07425-129">Request body</span></span>
<span data-ttu-id="07425-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07425-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07425-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="07425-131">Response</span></span>

<span data-ttu-id="07425-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07425-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07425-133">Пример</span><span class="sxs-lookup"><span data-stu-id="07425-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07425-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="07425-134">Request</span></span>
<span data-ttu-id="07425-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07425-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="07425-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="07425-136">Response</span></span>
<span data-ttu-id="07425-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07425-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
