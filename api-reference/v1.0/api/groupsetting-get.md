---
title: Получение параметра группы
description: Получение свойств для определенного объекта параметра группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d47441a66ab0b2ed3602a69f4a92a06050708f67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936503"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="2cedc-103">Получение параметра группы</span><span class="sxs-lookup"><span data-stu-id="2cedc-103">Get a group setting</span></span>

<span data-ttu-id="2cedc-104">Получение свойств для определенного объекта параметра группы.</span><span class="sxs-lookup"><span data-stu-id="2cedc-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cedc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cedc-105">Permissions</span></span>

<span data-ttu-id="2cedc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cedc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2cedc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cedc-108">Permission type</span></span>      | <span data-ttu-id="2cedc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cedc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cedc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cedc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2cedc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2cedc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2cedc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cedc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cedc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cedc-113">Not supported.</span></span>    |
|<span data-ttu-id="2cedc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cedc-114">Application</span></span> | <span data-ttu-id="2cedc-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cedc-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cedc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cedc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="2cedc-117">Получение указанного параметра, заданного на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="2cedc-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2cedc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2cedc-118">Optional query parameters</span></span>
<span data-ttu-id="2cedc-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2cedc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="2cedc-120">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cedc-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cedc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cedc-121">Request headers</span></span>
| <span data-ttu-id="2cedc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2cedc-122">Name</span></span> | <span data-ttu-id="2cedc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2cedc-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="2cedc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cedc-124">Authorization</span></span> | <span data-ttu-id="2cedc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cedc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cedc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cedc-127">Request body</span></span>

<span data-ttu-id="2cedc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cedc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cedc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cedc-129">Response</span></span>

<span data-ttu-id="2cedc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2cedc-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cedc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2cedc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cedc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cedc-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="2cedc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cedc-133">Response</span></span>

<span data-ttu-id="2cedc-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cedc-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
