---
title: Получение privilegedRoleAssignment
description: Извлечение свойств и связи объекта privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 12dd2587dc024deff48f678d44df4e2c876f02ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861378"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="406e2-103">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="406e2-103">Get privilegedRoleAssignment</span></span>

> <span data-ttu-id="406e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="406e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="406e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="406e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="406e2-106">Извлечение свойств и связи объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="406e2-106">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="406e2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="406e2-107">Permissions</span></span>
<span data-ttu-id="406e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="406e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="406e2-110">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="406e2-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="406e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="406e2-111">Permission type</span></span>      | <span data-ttu-id="406e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="406e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="406e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="406e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="406e2-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="406e2-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="406e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="406e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="406e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="406e2-116">Not supported.</span></span>    |
|<span data-ttu-id="406e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="406e2-117">Application</span></span> | <span data-ttu-id="406e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="406e2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="406e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="406e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="406e2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="406e2-120">Optional query parameters</span></span>
<span data-ttu-id="406e2-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="406e2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="406e2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="406e2-122">Request headers</span></span>
| <span data-ttu-id="406e2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="406e2-123">Name</span></span>      |<span data-ttu-id="406e2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="406e2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="406e2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="406e2-125">Authorization</span></span>  | <span data-ttu-id="406e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="406e2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="406e2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="406e2-128">Request body</span></span>
<span data-ttu-id="406e2-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="406e2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="406e2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="406e2-130">Response</span></span>

<span data-ttu-id="406e2-131">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="406e2-131">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="406e2-132">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="406e2-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="406e2-133">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="406e2-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="406e2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="406e2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="406e2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="406e2-135">Request</span></span>
<span data-ttu-id="406e2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="406e2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="406e2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="406e2-137">Response</span></span>
<span data-ttu-id="406e2-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="406e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
