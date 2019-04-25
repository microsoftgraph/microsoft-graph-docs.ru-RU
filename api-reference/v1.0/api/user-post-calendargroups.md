---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 775f499bc3fb5562f9936d7d64f20e5494f10bd0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563870"
---
# <a name="create-calendargroup"></a><span data-ttu-id="d3e36-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="d3e36-103">Create CalendarGroup</span></span>

<span data-ttu-id="d3e36-104">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="d3e36-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3e36-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e36-105">Permissions</span></span>
<span data-ttu-id="d3e36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e36-108">Permission type</span></span>      | <span data-ttu-id="d3e36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3e36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3e36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3e36-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e36-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d3e36-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3e36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e36-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e36-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d3e36-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3e36-114">Application</span></span> | <span data-ttu-id="d3e36-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e36-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3e36-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3e36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="d3e36-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3e36-117">Request headers</span></span>
| <span data-ttu-id="d3e36-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3e36-118">Header</span></span>       | <span data-ttu-id="d3e36-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d3e36-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3e36-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3e36-120">Authorization</span></span>  | <span data-ttu-id="d3e36-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3e36-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3e36-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3e36-123">Content-Type</span></span>  | <span data-ttu-id="d3e36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e36-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3e36-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3e36-125">Request body</span></span>
<span data-ttu-id="d3e36-126">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e36-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3e36-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e36-127">Response</span></span>

<span data-ttu-id="d3e36-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3e36-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e36-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d3e36-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3e36-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3e36-130">Request</span></span>
<span data-ttu-id="d3e36-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3e36-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="d3e36-132">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e36-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d3e36-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e36-133">Response</span></span>
<span data-ttu-id="d3e36-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3e36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
