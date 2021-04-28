---
title: List educationCategories
description: Извлечение списка объектов категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b4f821313796382b2bb7c9d5620dee96f463b227
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061793"
---
# <a name="list-educationcategories"></a><span data-ttu-id="f8c66-103">List educationCategories</span><span class="sxs-lookup"><span data-stu-id="f8c66-103">List educationCategories</span></span>

<span data-ttu-id="f8c66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8c66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c66-105">Извлечение списка [объектов educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f8c66-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8c66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8c66-106">Permissions</span></span>

<span data-ttu-id="f8c66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8c66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8c66-109">Permission type</span></span>                        | <span data-ttu-id="f8c66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8c66-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f8c66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8c66-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8c66-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8c66-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="f8c66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8c66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8c66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8c66-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="f8c66-115">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="f8c66-115">Application\*</span></span>                           | <span data-ttu-id="f8c66-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8c66-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="f8c66-117">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="f8c66-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="f8c66-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8c66-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8c66-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f8c66-119">Optional query parameters</span></span>

<span data-ttu-id="f8c66-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f8c66-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8c66-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8c66-121">Request headers</span></span>

| <span data-ttu-id="f8c66-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8c66-122">Header</span></span>        | <span data-ttu-id="f8c66-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f8c66-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="f8c66-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8c66-124">Authorization</span></span> | <span data-ttu-id="f8c66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8c66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8c66-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8c66-127">Request body</span></span>

<span data-ttu-id="f8c66-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8c66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8c66-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8c66-129">Response</span></span>

<span data-ttu-id="f8c66-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f8c66-130">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8c66-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8c66-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f8c66-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8c66-132">Request</span></span>

<span data-ttu-id="f8c66-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8c66-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="f8c66-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8c66-134">Response</span></span>

<span data-ttu-id="f8c66-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8c66-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f8c66-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f8c66-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
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