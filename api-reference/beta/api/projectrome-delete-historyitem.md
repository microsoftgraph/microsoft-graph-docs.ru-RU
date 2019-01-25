---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: b3e9a505c47c4d43aff71d5b4e40f08e3fe29d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520426"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="70990-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="70990-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70990-104">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="70990-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="70990-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70990-105">Permissions</span></span>

<span data-ttu-id="70990-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70990-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70990-108">Permission type</span></span>      | <span data-ttu-id="70990-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70990-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70990-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70990-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70990-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="70990-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="70990-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70990-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70990-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="70990-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="70990-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70990-114">Application</span></span> | <span data-ttu-id="70990-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70990-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70990-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70990-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70990-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70990-117">Request headers</span></span>

|<span data-ttu-id="70990-118">Имя</span><span class="sxs-lookup"><span data-stu-id="70990-118">Name</span></span> | <span data-ttu-id="70990-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70990-119">Type</span></span> | <span data-ttu-id="70990-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70990-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="70990-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70990-121">Authorization</span></span> | <span data-ttu-id="70990-122">string</span><span class="sxs-lookup"><span data-stu-id="70990-122">string</span></span> | <span data-ttu-id="70990-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70990-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70990-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70990-125">Request body</span></span>

<span data-ttu-id="70990-126">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="70990-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="70990-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="70990-127">Response</span></span>

<span data-ttu-id="70990-128">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если журнал элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="70990-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="70990-129">Пример</span><span class="sxs-lookup"><span data-stu-id="70990-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70990-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="70990-130">Request</span></span>

<span data-ttu-id="70990-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70990-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="70990-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="70990-132">Response</span></span>

<span data-ttu-id="70990-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70990-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
