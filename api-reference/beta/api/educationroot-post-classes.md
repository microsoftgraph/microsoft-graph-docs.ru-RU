---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этого API для создания класса он добавляет в группу специальные свойства, которые будут
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bdd0501e884aee897b52f92f85dd984fd85bff4b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007506"
---
# <a name="create-educationclass"></a><span data-ttu-id="393cb-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="393cb-105">Create educationClass</span></span>

<span data-ttu-id="393cb-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="393cb-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393cb-107">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="393cb-107">Create a new class.</span></span> <span data-ttu-id="393cb-108">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="393cb-108">This will also create a universal group.</span></span> <span data-ttu-id="393cb-109">При использовании этого API для создания класса в группу добавляются специальные свойства, в результате чего в Microsoft Teams добавляются такие функции, как назначения и специальная обработка в Microsoft Teams при создании Teams с помощью группы.</span><span class="sxs-lookup"><span data-stu-id="393cb-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="393cb-110">Обратите внимание, что этот API создает только универсальную группу и не создает команду.</span><span class="sxs-lookup"><span data-stu-id="393cb-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="393cb-111">Microsoft Teams предоставляет пользователям интерфейс для преподавателей, позволяющий создавать команды для собственных классов, используя группы, созданные этим API.</span><span class="sxs-lookup"><span data-stu-id="393cb-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="393cb-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="393cb-112">Permissions</span></span>
<span data-ttu-id="393cb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="393cb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="393cb-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="393cb-115">Permission type</span></span>      | <span data-ttu-id="393cb-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="393cb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="393cb-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="393cb-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="393cb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="393cb-118">Not supported.</span></span>  |
|<span data-ttu-id="393cb-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="393cb-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="393cb-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="393cb-120">Not supported.</span></span>  |
|<span data-ttu-id="393cb-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="393cb-121">Application</span></span> | <span data-ttu-id="393cb-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="393cb-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="393cb-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="393cb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="393cb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="393cb-124">Request headers</span></span>
| <span data-ttu-id="393cb-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="393cb-125">Header</span></span>       | <span data-ttu-id="393cb-126">Значение</span><span class="sxs-lookup"><span data-stu-id="393cb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="393cb-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="393cb-127">Authorization</span></span>  | <span data-ttu-id="393cb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="393cb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="393cb-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="393cb-130">Content-Type</span></span>  | <span data-ttu-id="393cb-131">application/json</span><span class="sxs-lookup"><span data-stu-id="393cb-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="393cb-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="393cb-132">Request body</span></span>
<span data-ttu-id="393cb-133">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="393cb-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="393cb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="393cb-134">Response</span></span>
<span data-ttu-id="393cb-135">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="393cb-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="393cb-136">Пример</span><span class="sxs-lookup"><span data-stu-id="393cb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="393cb-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="393cb-137">Request</span></span>
<span data-ttu-id="393cb-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="393cb-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="393cb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="393cb-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```
# <a name="c"></a>[<span data-ttu-id="393cb-140">C#</span><span class="sxs-lookup"><span data-stu-id="393cb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="393cb-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="393cb-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="393cb-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="393cb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="393cb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="393cb-143">Response</span></span>
<span data-ttu-id="393cb-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="393cb-144">The following is an example of the response.</span></span> 

><span data-ttu-id="393cb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="393cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


