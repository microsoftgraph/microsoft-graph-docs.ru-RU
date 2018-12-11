---
title: Список каналов
description: Получить список каналов в данной группы.
ms.openlocfilehash: 024751f0d77889249d2f2dcf6b2bb1f709128db1
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222543"
---
# <a name="list-channels"></a><span data-ttu-id="6e0bf-103">Список каналов</span><span class="sxs-lookup"><span data-stu-id="6e0bf-103">List channels</span></span>

> <span data-ttu-id="6e0bf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e0bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e0bf-106">Получить список [каналов](../resources/channel.md) из этой группы.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e0bf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e0bf-107">Permissions</span></span>
<span data-ttu-id="6e0bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e0bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6e0bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e0bf-110">Permission type</span></span>      | <span data-ttu-id="6e0bf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e0bf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e0bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e0bf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e0bf-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0bf-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e0bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e0bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e0bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-115">Not supported.</span></span>    |
|<span data-ttu-id="6e0bf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e0bf-116">Application</span></span> | <span data-ttu-id="6e0bf-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0bf-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6e0bf-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6e0bf-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e0bf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e0bf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e0bf-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e0bf-121">Optional query parameters</span></span>
<span data-ttu-id="6e0bf-122">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e0bf-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e0bf-123">Request headers</span></span>
| <span data-ttu-id="6e0bf-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e0bf-124">Header</span></span>       | <span data-ttu-id="6e0bf-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6e0bf-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e0bf-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e0bf-126">Authorization</span></span>  | <span data-ttu-id="6e0bf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e0bf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e0bf-129">Request body</span></span>
<span data-ttu-id="6e0bf-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e0bf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e0bf-131">Response</span></span>

<span data-ttu-id="6e0bf-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0bf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6e0bf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e0bf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e0bf-134">Request</span></span>
<span data-ttu-id="6e0bf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="6e0bf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e0bf-136">Response</span></span>
<span data-ttu-id="6e0bf-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e0bf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
