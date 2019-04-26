---
title: Получение объекта schedulingGroup
description: Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 008c131c2824bfb3d5b7e2b413858adb5ebc45ac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336144"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="57d18-103">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="57d18-103">Get schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57d18-104">Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="57d18-104">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="57d18-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57d18-105">Permissions</span></span>

<span data-ttu-id="57d18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d18-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d18-108">Permission type</span></span>      | <span data-ttu-id="57d18-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57d18-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d18-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57d18-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d18-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="57d18-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57d18-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d18-113">Not supported.</span></span>    |
|<span data-ttu-id="57d18-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57d18-114">Application</span></span> | <span data-ttu-id="57d18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d18-115">Not supported.</span></span> |

> <span data-ttu-id="57d18-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="57d18-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="57d18-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="57d18-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="57d18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d18-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="57d18-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57d18-119">Request headers</span></span>

| <span data-ttu-id="57d18-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57d18-120">Header</span></span>       | <span data-ttu-id="57d18-121">Значение</span><span class="sxs-lookup"><span data-stu-id="57d18-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57d18-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57d18-122">Authorization</span></span>  | <span data-ttu-id="57d18-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d18-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="57d18-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57d18-125">Content-Type</span></span>  | <span data-ttu-id="57d18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57d18-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57d18-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d18-127">Request body</span></span>
<span data-ttu-id="57d18-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57d18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57d18-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="57d18-129">Response</span></span>

<span data-ttu-id="57d18-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57d18-130">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57d18-131">Пример</span><span class="sxs-lookup"><span data-stu-id="57d18-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="57d18-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d18-132">Request</span></span>

<span data-ttu-id="57d18-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57d18-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="57d18-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d18-134">Response</span></span>

<span data-ttu-id="57d18-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57d18-135">The following is an example of the response.</span></span> 

><span data-ttu-id="57d18-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57d18-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
