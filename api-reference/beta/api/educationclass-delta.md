---
title: 'educationClass: Delta'
description: Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 03a026a479c9502e00b86e41936619613013b9af
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764773"
---
# <a name="educationclass-delta"></a><span data-ttu-id="bbb40-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="bbb40-103">educationClass: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbb40-104">Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.</span><span class="sxs-lookup"><span data-stu-id="bbb40-104">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="bbb40-105">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="bbb40-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbb40-106">Permissions</span></span>

<span data-ttu-id="bbb40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbb40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbb40-109">Permission type</span></span>                        | <span data-ttu-id="bbb40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbb40-110">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="bbb40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbb40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbb40-112">EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbb40-112">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="bbb40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbb40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbb40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb40-114">Not supported.</span></span>                                                           |
| <span data-ttu-id="bbb40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbb40-115">Application</span></span>                            | <span data-ttu-id="bbb40-116">EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="bbb40-116">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbb40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbb40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="bbb40-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbb40-118">Request headers</span></span>

| <span data-ttu-id="bbb40-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bbb40-119">Name</span></span>          | <span data-ttu-id="bbb40-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb40-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="bbb40-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbb40-121">Authorization</span></span> | <span data-ttu-id="bbb40-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bbb40-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbb40-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbb40-123">Request body</span></span>

<span data-ttu-id="bbb40-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbb40-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbb40-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbb40-125">Response</span></span>

<span data-ttu-id="bbb40-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationClass](../resources/educationclass.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbb40-126">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb40-127">Пример</span><span class="sxs-lookup"><span data-stu-id="bbb40-127">Example</span></span>

<span data-ttu-id="bbb40-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bbb40-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bbb40-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbb40-129">Request</span></span>

<span data-ttu-id="bbb40-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbb40-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="bbb40-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb40-131">Response</span></span>

<span data-ttu-id="bbb40-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbb40-132">The following is an example of the response.</span></span> 

><span data-ttu-id="bbb40-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbb40-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
