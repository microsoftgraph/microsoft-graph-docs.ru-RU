---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f69d29a1726545c6c0a85af2200294cfc1d6fe00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804525"
---
# <a name="add-a-student"></a><span data-ttu-id="07f64-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="07f64-103">Add a student</span></span>

<span data-ttu-id="07f64-104">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="07f64-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="07f64-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07f64-105">Permissions</span></span>
<span data-ttu-id="07f64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07f64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f64-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07f64-108">Permission type</span></span>      | <span data-ttu-id="07f64-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07f64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07f64-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07f64-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="07f64-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f64-111">Not supported.</span></span>  |
|<span data-ttu-id="07f64-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07f64-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="07f64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f64-113">Not supported.</span></span>  |
|<span data-ttu-id="07f64-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07f64-114">Application</span></span> | <span data-ttu-id="07f64-115">EduRoster.ReadWrite.All, а также Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="07f64-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="07f64-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07f64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="07f64-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07f64-117">Request headers</span></span>
| <span data-ttu-id="07f64-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07f64-118">Header</span></span>       | <span data-ttu-id="07f64-119">Значение</span><span class="sxs-lookup"><span data-stu-id="07f64-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07f64-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07f64-120">Authorization</span></span>  | <span data-ttu-id="07f64-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07f64-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07f64-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07f64-123">Content-Type</span></span>  | <span data-ttu-id="07f64-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07f64-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07f64-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07f64-125">Request body</span></span>
<span data-ttu-id="07f64-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07f64-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="07f64-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="07f64-127">Response</span></span>
<span data-ttu-id="07f64-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="07f64-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07f64-129">Пример</span><span class="sxs-lookup"><span data-stu-id="07f64-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07f64-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="07f64-130">Request</span></span>
<span data-ttu-id="07f64-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07f64-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="07f64-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="07f64-132">Response</span></span>
<span data-ttu-id="07f64-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="07f64-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
