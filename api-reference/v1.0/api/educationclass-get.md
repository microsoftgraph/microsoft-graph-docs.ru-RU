---
title: Получение educationClass
description: Извлечение класса из системы
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52f24e1f3c02b955874a78cdba447b697485f4a3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232013"
---
# <a name="get-educationclass"></a><span data-ttu-id="b5590-103">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="b5590-103">Get educationClass</span></span>

<span data-ttu-id="b5590-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5590-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5590-105">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="b5590-105">Retrieve a class from the system.</span></span> <span data-ttu-id="b5590-106">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="b5590-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="b5590-107">Участники группы представляют учащихся; Администраторы групп представляют преподавателей в классе.</span><span class="sxs-lookup"><span data-stu-id="b5590-107">Group members represent the students; group admins represent the teachers in the class.</span></span> <span data-ttu-id="b5590-108">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="b5590-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5590-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5590-109">Permissions</span></span>
<span data-ttu-id="b5590-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5590-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5590-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5590-112">Permission type</span></span>      | <span data-ttu-id="b5590-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5590-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5590-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5590-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b5590-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b5590-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b5590-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5590-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b5590-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5590-117">Not supported</span></span>  |
|<span data-ttu-id="b5590-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5590-118">Application</span></span> | <span data-ttu-id="b5590-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5590-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b5590-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5590-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5590-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5590-121">Optional query parameters</span></span>
<span data-ttu-id="b5590-122">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5590-122">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="b5590-123">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b5590-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5590-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5590-124">Request headers</span></span>
| <span data-ttu-id="b5590-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5590-125">Header</span></span>       | <span data-ttu-id="b5590-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b5590-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5590-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5590-127">Authorization</span></span>  | <span data-ttu-id="b5590-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5590-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5590-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5590-130">Request body</span></span>
<span data-ttu-id="b5590-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5590-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b5590-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5590-132">Response</span></span>
<span data-ttu-id="b5590-133">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5590-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5590-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b5590-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5590-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5590-135">Request</span></span>
<span data-ttu-id="b5590-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5590-136">Here is an example of the request.</span></span>

<span data-ttu-id="b5590-137">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5590-137">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5590-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5590-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5590-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5590-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```http
GET /education/classes/{educationClassId}
```

### <a name="response"></a><span data-ttu-id="b5590-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5590-140">Response</span></span>

><span data-ttu-id="b5590-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5590-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
    "displayName": "String",
    "mailNickname": "String",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "classCode": "String",
    "externalName": "String",
    "externalId": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "grade": "String",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm"
    }
  }
}
```
