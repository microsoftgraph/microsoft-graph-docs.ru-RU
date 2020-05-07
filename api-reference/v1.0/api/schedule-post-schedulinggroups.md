---
title: Создание объекта schedulingGroup
description: Создание нового Счедулингграуп.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92218b38d07c83acbd0e32893dce96fe9cf31286
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154716"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="5f950-103">Создание объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="5f950-103">Create schedulingGroup</span></span>

<span data-ttu-id="5f950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f950-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f950-105">Создание нового [счедулингграуп](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="5f950-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f950-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f950-106">Permissions</span></span>

<span data-ttu-id="5f950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f950-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f950-109">Permission type</span></span>      | <span data-ttu-id="5f950-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f950-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f950-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f950-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f950-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5f950-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f950-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f950-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f950-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f950-114">Not supported.</span></span>    |
|<span data-ttu-id="5f950-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f950-115">Application</span></span> |<span data-ttu-id="5f950-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f950-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="5f950-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="5f950-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5f950-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="5f950-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f950-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f950-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="5f950-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f950-120">Request headers</span></span>

| <span data-ttu-id="5f950-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f950-121">Header</span></span>       | <span data-ttu-id="5f950-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5f950-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f950-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f950-123">Authorization</span></span>  | <span data-ttu-id="5f950-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f950-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f950-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f950-126">Content-Type</span></span>  | <span data-ttu-id="5f950-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f950-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="5f950-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f950-129">Response</span></span>

<span data-ttu-id="5f950-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f950-130">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f950-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5f950-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f950-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f950-132">Request</span></span>

<span data-ttu-id="5f950-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f950-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
---


### <a name="response"></a><span data-ttu-id="5f950-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f950-134">Response</span></span>

<span data-ttu-id="5f950-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f950-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5f950-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f950-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
