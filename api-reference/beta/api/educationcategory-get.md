---
title: Get educationCategory
description: Извлечение объекта категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1c7dc80eb2e23dbf1fc09f9b906770b3b3a0fb47
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044090"
---
# <a name="get-educationcategory"></a><span data-ttu-id="cf5f3-103">Get educationCategory</span><span class="sxs-lookup"><span data-stu-id="cf5f3-103">Get educationCategory</span></span>

<span data-ttu-id="cf5f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf5f3-105">Извлечение [объекта educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="cf5f3-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf5f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5f3-106">Permissions</span></span>

<span data-ttu-id="cf5f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf5f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5f3-109">Permission type</span></span>                        | <span data-ttu-id="cf5f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf5f3-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cf5f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf5f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf5f3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf5f3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="cf5f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf5f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf5f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="cf5f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf5f3-115">Application</span></span>                            | <span data-ttu-id="cf5f3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf5f3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf5f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf5f3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf5f3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf5f3-118">Optional query parameters</span></span>

<span data-ttu-id="cf5f3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf5f3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf5f3-120">Request headers</span></span>
| <span data-ttu-id="cf5f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf5f3-121">Header</span></span>        | <span data-ttu-id="cf5f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf5f3-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cf5f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf5f3-123">Authorization</span></span> | <span data-ttu-id="cf5f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf5f3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf5f3-126">Request body</span></span>

<span data-ttu-id="cf5f3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf5f3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5f3-128">Response</span></span>

<span data-ttu-id="cf5f3-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5f3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cf5f3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf5f3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf5f3-131">Request</span></span>

<span data-ttu-id="cf5f3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="cf5f3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5f3-133">Response</span></span>

<span data-ttu-id="cf5f3-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-134">The following is an example of the response.</span></span>

><span data-ttu-id="cf5f3-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf5f3-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->