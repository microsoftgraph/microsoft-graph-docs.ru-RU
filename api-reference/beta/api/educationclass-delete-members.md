---
title: Удаление учащегося
description: Удаляет educationUser из educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac5ee332c58a070d9f25dfb3bde78177fb323b02
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324950"
---
# <a name="remove-a-student"></a><span data-ttu-id="b12a8-103">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="b12a8-103">Remove a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b12a8-104">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="b12a8-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="b12a8-105">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="b12a8-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="b12a8-106">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="b12a8-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="b12a8-107">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass-list-teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b12a8-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b12a8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b12a8-108">Permissions</span></span>
<span data-ttu-id="b12a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b12a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b12a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b12a8-111">Permission type</span></span>      | <span data-ttu-id="b12a8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b12a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b12a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b12a8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b12a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12a8-114">Not supported.</span></span>  |
|<span data-ttu-id="b12a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b12a8-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b12a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12a8-116">Not supported.</span></span>  |
|<span data-ttu-id="b12a8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b12a8-117">Application</span></span> | <span data-ttu-id="b12a8-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b12a8-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b12a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b12a8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b12a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b12a8-120">Request headers</span></span>
| <span data-ttu-id="b12a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b12a8-121">Header</span></span>       | <span data-ttu-id="b12a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b12a8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b12a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b12a8-123">Authorization</span></span>  | <span data-ttu-id="b12a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12a8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b12a8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b12a8-126">Request body</span></span>
<span data-ttu-id="b12a8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b12a8-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b12a8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b12a8-128">Response</span></span>
<span data-ttu-id="b12a8-129">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="b12a8-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b12a8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b12a8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b12a8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b12a8-131">Request</span></span>
<span data-ttu-id="b12a8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b12a8-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="b12a8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12a8-133">Response</span></span>
<span data-ttu-id="b12a8-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b12a8-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
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
