---
title: Добавление преподавателя
description: Добавление преподавателя в класс.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 959b873dba3f88665b170f52da4e4063adb200ae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507805"
---
# <a name="add-teacher"></a><span data-ttu-id="4e5b5-103">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="4e5b5-103">Add teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e5b5-104">Добавление преподавателя в класс.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e5b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e5b5-105">Permissions</span></span>
<span data-ttu-id="4e5b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e5b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e5b5-108">Permission type</span></span>      | <span data-ttu-id="4e5b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e5b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e5b5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-111">Not supported.</span></span>  |
|<span data-ttu-id="4e5b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e5b5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4e5b5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-113">Not supported.</span></span>  |
|<span data-ttu-id="4e5b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e5b5-114">Application</span></span> | <span data-ttu-id="4e5b5-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5b5-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4e5b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e5b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4e5b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e5b5-117">Request headers</span></span>
| <span data-ttu-id="4e5b5-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e5b5-118">Header</span></span>       | <span data-ttu-id="4e5b5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4e5b5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e5b5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e5b5-120">Authorization</span></span>  | <span data-ttu-id="4e5b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e5b5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e5b5-123">Content-Type</span></span>  | <span data-ttu-id="4e5b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4e5b5-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e5b5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e5b5-125">Request body</span></span>
<span data-ttu-id="4e5b5-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="4e5b5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e5b5-127">Response</span></span>
<span data-ttu-id="4e5b5-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e5b5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4e5b5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e5b5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e5b5-130">Request</span></span>
<span data-ttu-id="4e5b5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="4e5b5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e5b5-132">Response</span></span>
<span data-ttu-id="4e5b5-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="4e5b5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e5b5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-teachers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
