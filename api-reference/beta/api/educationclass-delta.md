---
title: 'educationClass: Delta'
description: Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 874898b68bcdb1d4bfc450668ebff89030859a02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426880"
---
# <a name="educationclass-delta"></a><span data-ttu-id="ec207-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="ec207-103">educationClass: delta</span></span>

<span data-ttu-id="ec207-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec207-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec207-105">Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.</span><span class="sxs-lookup"><span data-stu-id="ec207-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="ec207-106">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="ec207-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec207-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec207-107">Permissions</span></span>

<span data-ttu-id="ec207-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec207-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec207-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec207-110">Permission type</span></span>                        | <span data-ttu-id="ec207-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec207-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="ec207-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec207-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec207-113">EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec207-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="ec207-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec207-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec207-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec207-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="ec207-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec207-116">Application</span></span>                            | <span data-ttu-id="ec207-117">EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="ec207-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec207-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec207-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="ec207-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec207-119">Request headers</span></span>

| <span data-ttu-id="ec207-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec207-120">Name</span></span>          | <span data-ttu-id="ec207-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec207-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="ec207-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec207-122">Authorization</span></span> | <span data-ttu-id="ec207-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ec207-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec207-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec207-124">Request body</span></span>

<span data-ttu-id="ec207-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec207-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec207-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec207-126">Response</span></span>

<span data-ttu-id="ec207-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationClass](../resources/educationclass.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec207-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec207-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ec207-128">Example</span></span>

<span data-ttu-id="ec207-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ec207-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ec207-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec207-130">Request</span></span>

<span data-ttu-id="ec207-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec207-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="ec207-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec207-132">Response</span></span>

<span data-ttu-id="ec207-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec207-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ec207-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec207-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
