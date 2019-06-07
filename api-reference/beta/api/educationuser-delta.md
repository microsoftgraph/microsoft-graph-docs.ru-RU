---
title: 'educationUser: Delta'
description: Получите новых или обновленных пользователей, не требуя полного прочтения всей коллекции пользователей.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c89c065d5e4bd8510d6821a3c7a13bd106ce9eb8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764774"
---
# <a name="educationuser-delta"></a><span data-ttu-id="a3991-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="a3991-103">educationUser: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3991-104">Получите только что созданный или обновленный [educationUser](../resources/educationuser.md) , не требуя полного считывания всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="a3991-104">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="a3991-105">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="a3991-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3991-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3991-106">Permissions</span></span>

<span data-ttu-id="a3991-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3991-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3991-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3991-109">Permission type</span></span>                        | <span data-ttu-id="a3991-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3991-110">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="a3991-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3991-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3991-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3991-112">Not supported.</span></span>                                  |
| <span data-ttu-id="a3991-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3991-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3991-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3991-114">Not supported.</span></span>                                  |
| <span data-ttu-id="a3991-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3991-115">Application</span></span>                            | <span data-ttu-id="a3991-116">EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="a3991-116">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3991-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3991-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="a3991-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3991-118">Request headers</span></span>

| <span data-ttu-id="a3991-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a3991-119">Name</span></span>          | <span data-ttu-id="a3991-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3991-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="a3991-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3991-121">Authorization</span></span> | <span data-ttu-id="a3991-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a3991-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3991-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3991-123">Request body</span></span>

<span data-ttu-id="a3991-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3991-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3991-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3991-125">Response</span></span>

<span data-ttu-id="a3991-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationUser](../resources/educationuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3991-126">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3991-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a3991-127">Example</span></span>

<span data-ttu-id="a3991-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a3991-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a3991-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3991-129">Request</span></span>

<span data-ttu-id="a3991-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3991-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="a3991-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3991-131">Response</span></span>

<span data-ttu-id="a3991-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3991-132">The following is an example of the response.</span></span>

><span data-ttu-id="a3991-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3991-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
