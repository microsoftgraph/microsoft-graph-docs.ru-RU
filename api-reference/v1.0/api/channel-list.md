---
title: Список каналов
description: Получить список каналов в данной группы.
ms.openlocfilehash: 5f96d4c47a787839626a9d90733d087906407b01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025860"
---
# <a name="list-channels"></a><span data-ttu-id="1a134-103">Список каналов</span><span class="sxs-lookup"><span data-stu-id="1a134-103">List channels</span></span>



<span data-ttu-id="1a134-104">Получить список [каналов](../resources/channel.md) из этой группы.</span><span class="sxs-lookup"><span data-stu-id="1a134-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a134-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a134-105">Permissions</span></span>
<span data-ttu-id="1a134-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a134-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a134-108">Permission type</span></span>      | <span data-ttu-id="1a134-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a134-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a134-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a134-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a134-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a134-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a134-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a134-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a134-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a134-113">Not supported.</span></span>    |
|<span data-ttu-id="1a134-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a134-114">Application</span></span> | <span data-ttu-id="1a134-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a134-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="1a134-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a134-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a134-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a134-117">Optional query parameters</span></span>
<span data-ttu-id="1a134-118">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a134-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a134-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a134-119">Request headers</span></span>
| <span data-ttu-id="1a134-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a134-120">Header</span></span>       | <span data-ttu-id="1a134-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a134-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a134-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a134-122">Authorization</span></span>  | <span data-ttu-id="1a134-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a134-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a134-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a134-125">Request body</span></span>
<span data-ttu-id="1a134-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a134-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a134-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a134-127">Response</span></span>

<span data-ttu-id="1a134-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1a134-128">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a134-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1a134-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a134-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a134-130">Request</span></span>
<span data-ttu-id="1a134-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a134-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="1a134-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a134-132">Response</span></span>
<span data-ttu-id="1a134-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1a134-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
