---
title: Получение объекта schedulingGroup
description: Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f58d41c588c9937645480d3d0f5075c9753fda17
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154194"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="3f81c-103">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="3f81c-103">Get schedulingGroup</span></span>

<span data-ttu-id="3f81c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f81c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f81c-105">Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="3f81c-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f81c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f81c-106">Permissions</span></span>

<span data-ttu-id="3f81c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f81c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f81c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f81c-109">Permission type</span></span>      | <span data-ttu-id="3f81c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f81c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f81c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f81c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f81c-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f81c-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f81c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f81c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f81c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f81c-114">Not supported.</span></span>    |
|<span data-ttu-id="3f81c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f81c-115">Application</span></span> | <span data-ttu-id="3f81c-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f81c-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |


> <span data-ttu-id="3f81c-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3f81c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3f81c-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="3f81c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3f81c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f81c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f81c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3f81c-120">Optional query parameters</span></span>

<span data-ttu-id="3f81c-121">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3f81c-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f81c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f81c-122">Request headers</span></span>

| <span data-ttu-id="3f81c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f81c-123">Header</span></span>       | <span data-ttu-id="3f81c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3f81c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f81c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f81c-125">Authorization</span></span>  | <span data-ttu-id="3f81c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f81c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f81c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f81c-128">Request body</span></span>
<span data-ttu-id="3f81c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f81c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f81c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f81c-130">Response</span></span>

<span data-ttu-id="3f81c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f81c-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f81c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3f81c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f81c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f81c-133">Request</span></span>

<span data-ttu-id="3f81c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f81c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="3f81c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f81c-135">Response</span></span>

<span data-ttu-id="3f81c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f81c-136">The following is an example of the response.</span></span> 

><span data-ttu-id="3f81c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f81c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
