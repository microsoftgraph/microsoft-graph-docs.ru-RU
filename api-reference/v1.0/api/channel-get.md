---
title: Получение канала
description: Извлечение свойств и связи канала.
ms.openlocfilehash: fd46e3f27c9da53a36107c3ec39c1ac5da1c0753
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222424"
---
# <a name="get-channel"></a><span data-ttu-id="19599-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="19599-103">Get channel</span></span>



<span data-ttu-id="19599-104">Извлечение свойств и связи [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="19599-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="19599-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19599-105">Permissions</span></span>
<span data-ttu-id="19599-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19599-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19599-108">Permission type</span></span>      | <span data-ttu-id="19599-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19599-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19599-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19599-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19599-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19599-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="19599-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19599-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19599-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19599-113">Not supported.</span></span>    |
|<span data-ttu-id="19599-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19599-114">Application</span></span> | <span data-ttu-id="19599-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19599-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="19599-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="19599-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="19599-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="19599-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="19599-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19599-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="19599-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19599-119">Optional query parameters</span></span>

<span data-ttu-id="19599-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19599-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19599-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19599-121">Request headers</span></span>
| <span data-ttu-id="19599-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19599-122">Header</span></span>       | <span data-ttu-id="19599-123">Значение</span><span class="sxs-lookup"><span data-stu-id="19599-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19599-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19599-124">Authorization</span></span>  | <span data-ttu-id="19599-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19599-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19599-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19599-127">Request body</span></span>
<span data-ttu-id="19599-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19599-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19599-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="19599-129">Response</span></span>

<span data-ttu-id="19599-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19599-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19599-131">Пример</span><span class="sxs-lookup"><span data-stu-id="19599-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19599-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="19599-132">Request</span></span>
<span data-ttu-id="19599-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19599-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="19599-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="19599-134">Response</span></span>
<span data-ttu-id="19599-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19599-135">Here is an example of the response.</span></span> 

><span data-ttu-id="19599-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19599-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
