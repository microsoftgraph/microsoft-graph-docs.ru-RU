---
title: Получение educationClass
description: "  Группа \"Администраторы\" представляют преподавателей в классе. Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является."
localization_priority: Normal
ms.openlocfilehash: 9d4a48a12d05bd7ef6bd1c6204ce23755b26019e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874930"
---
# <a name="get-educationclass"></a><span data-ttu-id="35a44-104">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="35a44-104">Get educationClass</span></span>

> <span data-ttu-id="35a44-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35a44-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35a44-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35a44-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35a44-107">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="35a44-107">Retrieve a class from the system.</span></span> <span data-ttu-id="35a44-108">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="35a44-108">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="35a44-109">Члены группы представляют учащихся, администраторы группы — преподавателей курса.</span><span class="sxs-lookup"><span data-stu-id="35a44-109">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="35a44-110">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="35a44-110">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="35a44-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35a44-111">Permissions</span></span>
<span data-ttu-id="35a44-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35a44-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35a44-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35a44-114">Permission type</span></span>      | <span data-ttu-id="35a44-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35a44-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35a44-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35a44-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="35a44-117">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="35a44-117">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="35a44-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35a44-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="35a44-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="35a44-119">Not supported</span></span>  |
|<span data-ttu-id="35a44-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35a44-120">Application</span></span> | <span data-ttu-id="35a44-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35a44-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="35a44-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35a44-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35a44-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35a44-123">Optional query parameters</span></span>
<span data-ttu-id="35a44-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35a44-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35a44-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35a44-125">Request headers</span></span>
| <span data-ttu-id="35a44-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35a44-126">Header</span></span>       | <span data-ttu-id="35a44-127">Значение</span><span class="sxs-lookup"><span data-stu-id="35a44-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35a44-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35a44-128">Authorization</span></span>  | <span data-ttu-id="35a44-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35a44-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35a44-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35a44-131">Request body</span></span>
<span data-ttu-id="35a44-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35a44-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="35a44-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="35a44-133">Response</span></span>
<span data-ttu-id="35a44-134">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35a44-134">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35a44-135">Пример</span><span class="sxs-lookup"><span data-stu-id="35a44-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35a44-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="35a44-136">Request</span></span>
<span data-ttu-id="35a44-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35a44-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="35a44-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="35a44-138">Response</span></span>
<span data-ttu-id="35a44-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35a44-139">The following is an example of the response.</span></span> 

><span data-ttu-id="35a44-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35a44-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
