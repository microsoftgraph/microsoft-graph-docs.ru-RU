---
title: Получение educationClass
description: "  Группа \"Администраторы\" представляют преподавателей в классе. Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является."
localization_priority: Normal
ms.openlocfilehash: 56717404d996e04c57ff194dafdb8231cf96f55f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849590"
---
# <a name="get-educationclass"></a><span data-ttu-id="deb32-104">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="deb32-104">Get educationClass</span></span>

<span data-ttu-id="deb32-105">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="deb32-105">Retrieve a class from the system.</span></span> <span data-ttu-id="deb32-106">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="deb32-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="deb32-107">Члены группы представляют учащихся, администраторы группы — преподавателей курса.</span><span class="sxs-lookup"><span data-stu-id="deb32-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="deb32-108">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="deb32-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb32-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deb32-109">Permissions</span></span>
<span data-ttu-id="deb32-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb32-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb32-112">Permission type</span></span>      | <span data-ttu-id="deb32-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb32-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deb32-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb32-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="deb32-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="deb32-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="deb32-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb32-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="deb32-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="deb32-117">Not supported</span></span>  |
|<span data-ttu-id="deb32-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb32-118">Application</span></span> | <span data-ttu-id="deb32-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb32-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="deb32-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb32-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="deb32-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="deb32-121">Optional query parameters</span></span>
<span data-ttu-id="deb32-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="deb32-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deb32-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deb32-123">Request headers</span></span>
| <span data-ttu-id="deb32-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="deb32-124">Header</span></span>       | <span data-ttu-id="deb32-125">Значение</span><span class="sxs-lookup"><span data-stu-id="deb32-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="deb32-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deb32-126">Authorization</span></span>  | <span data-ttu-id="deb32-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb32-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="deb32-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="deb32-129">Request body</span></span>
<span data-ttu-id="deb32-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="deb32-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="deb32-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb32-131">Response</span></span>
<span data-ttu-id="deb32-132">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="deb32-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="deb32-133">Пример</span><span class="sxs-lookup"><span data-stu-id="deb32-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="deb32-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb32-134">Request</span></span>
<span data-ttu-id="deb32-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb32-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="deb32-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="deb32-136">Response</span></span>
<span data-ttu-id="deb32-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="deb32-137">The following is an example of the response.</span></span> 

><span data-ttu-id="deb32-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="deb32-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
