---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: fe950190ce3bd56b5f236f42a840d3d0b9f5d130
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960926"
---
# <a name="list-classes"></a><span data-ttu-id="dbb5b-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="dbb5b-104">List classes</span></span>

> <span data-ttu-id="dbb5b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbb5b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbb5b-107">Получение списка объектов курсов.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-107">Retrieve a list of class objects.</span></span> <span data-ttu-id="dbb5b-108">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-108">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="dbb5b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbb5b-109">Permissions</span></span>
<span data-ttu-id="dbb5b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb5b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb5b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbb5b-112">Permission type</span></span>      | <span data-ttu-id="dbb5b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbb5b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbb5b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbb5b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="dbb5b-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="dbb5b-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="dbb5b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbb5b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dbb5b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-117">Not supported.</span></span>  |
|<span data-ttu-id="dbb5b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbb5b-118">Application</span></span> | <span data-ttu-id="dbb5b-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb5b-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dbb5b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbb5b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbb5b-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dbb5b-121">Optional query parameters</span></span>
<span data-ttu-id="dbb5b-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbb5b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbb5b-123">Request headers</span></span>
| <span data-ttu-id="dbb5b-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbb5b-124">Header</span></span>       | <span data-ttu-id="dbb5b-125">Значение</span><span class="sxs-lookup"><span data-stu-id="dbb5b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbb5b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbb5b-126">Authorization</span></span>  | <span data-ttu-id="dbb5b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbb5b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbb5b-129">Request body</span></span>
<span data-ttu-id="dbb5b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dbb5b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbb5b-131">Response</span></span>
<span data-ttu-id="dbb5b-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-132">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbb5b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dbb5b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbb5b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbb5b-134">Request</span></span>
<span data-ttu-id="dbb5b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="dbb5b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbb5b-136">Response</span></span>
<span data-ttu-id="dbb5b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-137">The following is an example of the response.</span></span> 

><span data-ttu-id="dbb5b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbb5b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
