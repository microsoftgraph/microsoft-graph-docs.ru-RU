---
title: Замена объекта schedulingGroup
description: Замена существующего Счедулингграуп.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c56fc696469cce89a82d4dd9a46ef6d61e07e495
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154187"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="10638-103">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="10638-103">Replace schedulingGroup</span></span>

<span data-ttu-id="10638-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10638-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10638-105">Замена существующего [счедулингграуп](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="10638-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="10638-106">Если указанный [счедулингграуп](../resources/schedulinggroup.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="10638-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="10638-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10638-107">Permissions</span></span>

<span data-ttu-id="10638-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10638-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10638-110">Permission type</span></span>      | <span data-ttu-id="10638-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10638-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10638-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10638-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10638-113">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10638-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="10638-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10638-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10638-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10638-115">Not supported.</span></span>    |
|<span data-ttu-id="10638-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10638-116">Application</span></span> | <span data-ttu-id="10638-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10638-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="10638-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="10638-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="10638-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="10638-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="10638-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10638-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="10638-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10638-121">Request headers</span></span>

| <span data-ttu-id="10638-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10638-122">Header</span></span>       | <span data-ttu-id="10638-123">Значение</span><span class="sxs-lookup"><span data-stu-id="10638-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10638-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10638-124">Authorization</span></span>  | <span data-ttu-id="10638-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10638-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10638-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10638-127">Content-Type</span></span>  | <span data-ttu-id="10638-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10638-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10638-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10638-130">Request body</span></span>

<span data-ttu-id="10638-131">В тексте запроса добавьте представление объекта [счедулингграуп](../resources/schedulinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10638-131">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10638-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="10638-132">Response</span></span>

<span data-ttu-id="10638-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10638-133">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10638-134">Пример</span><span class="sxs-lookup"><span data-stu-id="10638-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="10638-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="10638-135">Request</span></span>

<span data-ttu-id="10638-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10638-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Prefer: return=representation

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


### <a name="response"></a><span data-ttu-id="10638-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10638-137">Response</span></span>

<span data-ttu-id="10638-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10638-138">The following is an example of the response.</span></span> 

><span data-ttu-id="10638-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10638-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Replace an existing schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
