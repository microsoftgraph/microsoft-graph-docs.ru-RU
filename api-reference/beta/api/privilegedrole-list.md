---
title: Список privilegedRoles
description: Получение списка объектов privilegedRole.
localization_priority: Normal
ms.openlocfilehash: c36ea34cc6d7ee1999e37f15eff543f48bbfc2bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826049"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="913bc-103">Список privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="913bc-103">List privilegedRoles</span></span>

> <span data-ttu-id="913bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="913bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="913bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="913bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="913bc-106">Получение списка объектов [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="913bc-106">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="913bc-107">Чтобы отфильтровать результаты запроса, используйте стандартные OData ``$filter`` выражения в URI.</span><span class="sxs-lookup"><span data-stu-id="913bc-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="913bc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="913bc-108">Permissions</span></span>
<span data-ttu-id="913bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="913bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="913bc-111">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="913bc-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="913bc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="913bc-112">Permission type</span></span>      | <span data-ttu-id="913bc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="913bc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="913bc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="913bc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="913bc-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="913bc-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="913bc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="913bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="913bc-117">Not supported.</span></span>    |
|<span data-ttu-id="913bc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="913bc-118">Application</span></span> | <span data-ttu-id="913bc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="913bc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="913bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="913bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="913bc-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="913bc-121">Optional query parameters</span></span>
<span data-ttu-id="913bc-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="913bc-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="913bc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="913bc-123">Request headers</span></span>
| <span data-ttu-id="913bc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="913bc-124">Name</span></span>      |<span data-ttu-id="913bc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="913bc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="913bc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="913bc-126">Authorization</span></span>  | <span data-ttu-id="913bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="913bc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="913bc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="913bc-129">Request body</span></span>
<span data-ttu-id="913bc-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="913bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="913bc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="913bc-131">Response</span></span>

<span data-ttu-id="913bc-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRole](../resources/privilegedrole.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="913bc-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="913bc-133">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="913bc-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="913bc-134">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="913bc-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="913bc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="913bc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="913bc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="913bc-136">Request</span></span>
<span data-ttu-id="913bc-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="913bc-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="913bc-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="913bc-138">Response</span></span>
<span data-ttu-id="913bc-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="913bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
