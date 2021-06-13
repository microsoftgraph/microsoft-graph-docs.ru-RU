---
title: Назначение спискаCategories
description: Извлечение списка объектов категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3f7851e746cb87905768604610cd17d036cc963c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911839"
---
# <a name="list-assignmentcategories"></a><span data-ttu-id="2d04e-103">Назначение спискаCategories</span><span class="sxs-lookup"><span data-stu-id="2d04e-103">List assignmentCategories</span></span>

<span data-ttu-id="2d04e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d04e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d04e-105">Извлечение списка [объектов educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2d04e-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d04e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d04e-106">Permissions</span></span>

<span data-ttu-id="2d04e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d04e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d04e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d04e-109">Permission type</span></span>                        | <span data-ttu-id="2d04e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d04e-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2d04e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d04e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d04e-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d04e-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2d04e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d04e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d04e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d04e-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="2d04e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d04e-115">Application</span></span>                            | <span data-ttu-id="2d04e-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d04e-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d04e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d04e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d04e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d04e-118">Optional query parameters</span></span>

<span data-ttu-id="2d04e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2d04e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d04e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d04e-120">Request headers</span></span>

| <span data-ttu-id="2d04e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d04e-121">Header</span></span>        | <span data-ttu-id="2d04e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2d04e-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2d04e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d04e-123">Authorization</span></span> | <span data-ttu-id="2d04e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d04e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d04e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d04e-126">Request body</span></span>

<span data-ttu-id="2d04e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d04e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d04e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d04e-128">Response</span></span>

<span data-ttu-id="2d04e-129">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2d04e-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d04e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d04e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2d04e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d04e-131">Request</span></span>

<span data-ttu-id="2d04e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d04e-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["4797d052-ebf5-4018-a088-e11adc6b2cbb"],
  "name": "get_class_categories"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="2d04e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d04e-133">Response</span></span>

<span data-ttu-id="2d04e-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d04e-134">The following is an example of the response.</span></span> 

><span data-ttu-id="2d04e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d04e-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('4797d052-ebf5-4018-a088-e11adc6b2cbb')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
          "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
