---
title: Создание объекта Attachment
description: Используйте этот интерфейс API для добавления вложения в outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ae6c420c9c0ccf10df4d2d62a27f4b8c0d857c32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525026"
---
# <a name="create-attachment"></a><span data-ttu-id="3272f-103">Создание вложения</span><span class="sxs-lookup"><span data-stu-id="3272f-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3272f-104">Используйте этот интерфейс API для добавления [вложений](../resources/attachment.md) к [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="3272f-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3272f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3272f-105">Permissions</span></span>

<span data-ttu-id="3272f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3272f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3272f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3272f-108">Permission type</span></span>      | <span data-ttu-id="3272f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3272f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3272f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3272f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3272f-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3272f-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3272f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3272f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3272f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3272f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3272f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3272f-114">Application</span></span> | <span data-ttu-id="3272f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3272f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3272f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3272f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="3272f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3272f-117">Request headers</span></span>

| <span data-ttu-id="3272f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3272f-118">Name</span></span>       | <span data-ttu-id="3272f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3272f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3272f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3272f-120">Authorization</span></span>  | <span data-ttu-id="3272f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3272f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3272f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3272f-123">Content-Type</span></span> | <span data-ttu-id="3272f-124">Строка, представляющая тип данных в теле сущности.</span><span class="sxs-lookup"><span data-stu-id="3272f-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="3272f-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3272f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3272f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3272f-126">Request body</span></span>

<span data-ttu-id="3272f-127">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3272f-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3272f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3272f-128">Response</span></span>

<span data-ttu-id="3272f-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3272f-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3272f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3272f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3272f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3272f-131">Request</span></span>

<span data-ttu-id="3272f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3272f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```

### <a name="response"></a><span data-ttu-id="3272f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3272f-133">Response</span></span>

<span data-ttu-id="3272f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3272f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
