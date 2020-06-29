---
title: 'educationUser: Delta'
description: Получите новых или обновленных пользователей, не требуя полного прочтения всей коллекции пользователей.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 408fb43dbad69cbb699db899522cf938e84ec904
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909559"
---
# <a name="educationuser-delta"></a><span data-ttu-id="3603c-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="3603c-103">educationUser: delta</span></span>

<span data-ttu-id="3603c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3603c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3603c-105">Получите только что созданный или обновленный [educationUser](../resources/educationuser.md) , не требуя полного считывания всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="3603c-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="3603c-106">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="3603c-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="3603c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3603c-107">Permissions</span></span>

<span data-ttu-id="3603c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3603c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3603c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3603c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3603c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3603c-110">Permission type</span></span>                        | <span data-ttu-id="3603c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3603c-111">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="3603c-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3603c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3603c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3603c-113">Not supported.</span></span>                                  |
| <span data-ttu-id="3603c-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3603c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3603c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3603c-115">Not supported.</span></span>                                  |
| <span data-ttu-id="3603c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3603c-116">Application</span></span>                            | <span data-ttu-id="3603c-117">EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="3603c-117">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3603c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3603c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="3603c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3603c-119">Request headers</span></span>

| <span data-ttu-id="3603c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3603c-120">Name</span></span>          | <span data-ttu-id="3603c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3603c-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="3603c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3603c-122">Authorization</span></span> | <span data-ttu-id="3603c-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3603c-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3603c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3603c-124">Request body</span></span>

<span data-ttu-id="3603c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3603c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3603c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3603c-126">Response</span></span>

<span data-ttu-id="3603c-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationUser](../resources/educationuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3603c-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3603c-128">разность educationUser не включает удаленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3603c-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="3603c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3603c-129">Example</span></span>

<span data-ttu-id="3603c-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3603c-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3603c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3603c-131">Request</span></span>

<span data-ttu-id="3603c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3603c-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="3603c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3603c-133">Response</span></span>

<span data-ttu-id="3603c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3603c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="3603c-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="3603c-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3603c-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3603c-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "primaryRole": "primaryRole-value",
      "middleName": "middleName-value",
      "externalSource": "externalSource-value",
      "residenceAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "mailingAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "student": {
        "graduationYear": "graduationYear-value",
        "grade": "grade-value",
        "birthDate": "datetime-value",
        "gender": "gender-value",
        "studentNumber": "studentNumber-value",
        "externalId": "externalId-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
