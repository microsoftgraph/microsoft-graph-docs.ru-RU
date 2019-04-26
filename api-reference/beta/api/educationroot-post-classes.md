---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этого API для создания класса он добавляет в группу специальные свойства, которые будут
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 50b5cfcffdf6509d5da13a12dbf1829fde5e2420
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324847"
---
# <a name="create-educationclass"></a><span data-ttu-id="e175e-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="e175e-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e175e-106">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="e175e-106">Create a new class.</span></span> <span data-ttu-id="e175e-107">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="e175e-107">This will also create a universal group.</span></span> <span data-ttu-id="e175e-108">Если вы используете этот API для создания курса, он добавит специальные свойства в группу, что приведет к добавлению возможностей, таких как задания и специальная обработка в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e175e-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="e175e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e175e-109">Permissions</span></span>
<span data-ttu-id="e175e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e175e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e175e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e175e-112">Permission type</span></span>      | <span data-ttu-id="e175e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e175e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e175e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e175e-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e175e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e175e-115">Not supported.</span></span>  |
|<span data-ttu-id="e175e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e175e-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e175e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e175e-117">Not supported.</span></span>  |
|<span data-ttu-id="e175e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="e175e-118">Application</span></span> | <span data-ttu-id="e175e-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e175e-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e175e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e175e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="e175e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e175e-121">Request headers</span></span>
| <span data-ttu-id="e175e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e175e-122">Header</span></span>       | <span data-ttu-id="e175e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e175e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e175e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e175e-124">Authorization</span></span>  | <span data-ttu-id="e175e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e175e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e175e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e175e-127">Content-Type</span></span>  | <span data-ttu-id="e175e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e175e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e175e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e175e-129">Request body</span></span>
<span data-ttu-id="e175e-130">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e175e-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e175e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e175e-131">Response</span></span>
<span data-ttu-id="e175e-132">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e175e-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e175e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e175e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e175e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e175e-134">Request</span></span>
<span data-ttu-id="e175e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e175e-135">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e175e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e175e-136">Response</span></span>
<span data-ttu-id="e175e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e175e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e175e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e175e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
