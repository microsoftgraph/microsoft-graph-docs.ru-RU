---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этот интерфейс API для создания класса специальные свойства добавляется в группу, которая будет
ms.openlocfilehash: 81b72b5b252c323a6a91152deaafaf8a927c8bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074695"
---
# <a name="create-educationclass"></a><span data-ttu-id="47566-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="47566-105">Create educationClass</span></span>

> <span data-ttu-id="47566-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47566-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47566-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47566-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47566-108">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="47566-108">Create a new class.</span></span> <span data-ttu-id="47566-109">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="47566-109">This will also create a universal group.</span></span> <span data-ttu-id="47566-110">Если вы используете этот API для создания курса, он добавит специальные свойства в группу, что приведет к добавлению возможностей, таких как задания и специальная обработка в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="47566-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="47566-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47566-111">Permissions</span></span>
<span data-ttu-id="47566-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47566-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47566-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47566-114">Permission type</span></span>      | <span data-ttu-id="47566-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47566-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47566-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47566-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="47566-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47566-117">Not supported.</span></span>  |
|<span data-ttu-id="47566-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47566-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47566-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47566-119">Not supported.</span></span>  |
|<span data-ttu-id="47566-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47566-120">Application</span></span> | <span data-ttu-id="47566-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47566-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47566-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47566-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="47566-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47566-123">Request headers</span></span>
| <span data-ttu-id="47566-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47566-124">Header</span></span>       | <span data-ttu-id="47566-125">Значение</span><span class="sxs-lookup"><span data-stu-id="47566-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47566-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47566-126">Authorization</span></span>  | <span data-ttu-id="47566-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47566-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="47566-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47566-129">Content-Type</span></span>  | <span data-ttu-id="47566-130">application/json</span><span class="sxs-lookup"><span data-stu-id="47566-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47566-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47566-131">Request body</span></span>
<span data-ttu-id="47566-132">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47566-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="47566-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="47566-133">Response</span></span>
<span data-ttu-id="47566-134">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47566-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47566-135">Пример</span><span class="sxs-lookup"><span data-stu-id="47566-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47566-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="47566-136">Request</span></span>
<span data-ttu-id="47566-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47566-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="47566-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="47566-138">Response</span></span>
<span data-ttu-id="47566-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47566-139">The following is an example of the response.</span></span> 

><span data-ttu-id="47566-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47566-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->