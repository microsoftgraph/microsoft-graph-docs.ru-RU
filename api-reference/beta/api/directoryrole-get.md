---
title: Получение объекта directoryRole
description: Получение свойств объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: bb438f2362c7f6c7d95dd0b1952bac29aa21616a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859152"
---
# <a name="get-directoryrole"></a><span data-ttu-id="f2b49-103">Получение объекта directoryRole</span><span class="sxs-lookup"><span data-stu-id="f2b49-103">Get directoryRole</span></span>

> <span data-ttu-id="f2b49-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2b49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2b49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b49-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2b49-106">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="f2b49-106">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2b49-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b49-107">Permissions</span></span>
<span data-ttu-id="f2b49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b49-110">Permission type</span></span>      | <span data-ttu-id="f2b49-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2b49-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2b49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2b49-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2b49-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2b49-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2b49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2b49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2b49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b49-115">Not supported.</span></span>    |
|<span data-ttu-id="f2b49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2b49-116">Application</span></span> | <span data-ttu-id="f2b49-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b49-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2b49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2b49-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2b49-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2b49-119">Optional query parameters</span></span>
<span data-ttu-id="f2b49-120">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="f2b49-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2b49-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2b49-121">Request headers</span></span>
| <span data-ttu-id="f2b49-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2b49-122">Name</span></span>       | <span data-ttu-id="f2b49-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f2b49-123">Type</span></span> | <span data-ttu-id="f2b49-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b49-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2b49-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b49-125">Authorization</span></span>  | <span data-ttu-id="f2b49-126">string</span><span class="sxs-lookup"><span data-stu-id="f2b49-126">string</span></span>  | <span data-ttu-id="f2b49-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2b49-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2b49-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2b49-129">Request body</span></span>
<span data-ttu-id="f2b49-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2b49-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2b49-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b49-131">Response</span></span>

<span data-ttu-id="f2b49-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2b49-132">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2b49-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f2b49-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2b49-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2b49-134">Request</span></span>
<span data-ttu-id="f2b49-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2b49-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="f2b49-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2b49-136">Response</span></span>
<span data-ttu-id="f2b49-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f2b49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
