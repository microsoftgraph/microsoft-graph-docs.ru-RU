---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
ms.openlocfilehash: 523a9245c57878dc618b778b968d28c41fc7cd45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025045"
---
# <a name="create-calendargroup"></a><span data-ttu-id="b9cc9-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="b9cc9-103">Create CalendarGroup</span></span>

<span data-ttu-id="b9cc9-104">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9cc9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9cc9-105">Permissions</span></span>
<span data-ttu-id="b9cc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cc9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9cc9-108">Permission type</span></span>      | <span data-ttu-id="b9cc9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9cc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9cc9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9cc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9cc9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9cc9-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b9cc9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9cc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9cc9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9cc9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b9cc9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9cc9-114">Application</span></span> | <span data-ttu-id="b9cc9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9cc9-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9cc9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9cc9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="b9cc9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9cc9-117">Request headers</span></span>
| <span data-ttu-id="b9cc9-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9cc9-118">Header</span></span>       | <span data-ttu-id="b9cc9-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b9cc9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9cc9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9cc9-120">Authorization</span></span>  | <span data-ttu-id="b9cc9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9cc9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9cc9-123">Content-Type</span></span>  | <span data-ttu-id="b9cc9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b9cc9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9cc9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9cc9-125">Request body</span></span>
<span data-ttu-id="b9cc9-126">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b9cc9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9cc9-127">Response</span></span>

<span data-ttu-id="b9cc9-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9cc9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b9cc9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9cc9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9cc9-130">Request</span></span>
<span data-ttu-id="b9cc9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="b9cc9-132">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cc9-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b9cc9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9cc9-133">Response</span></span>
<span data-ttu-id="b9cc9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b9cc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
