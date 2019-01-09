---
title: Создать подключение
description: Используйте этот интерфейс API для добавления вложения в outlookTask.
author: angelgolfer-ms
ms.openlocfilehash: 3b3cc5d6d4357e74c0b63166a492eafe97813b06
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771676"
---
# <a name="create-attachment"></a><span data-ttu-id="7f599-103">Создание вложения</span><span class="sxs-lookup"><span data-stu-id="7f599-103">Create attachment</span></span>

> <span data-ttu-id="7f599-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f599-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f599-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f599-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f599-106">Используйте этот интерфейс API для добавления [вложений](../resources/attachment.md) к [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="7f599-106">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f599-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f599-107">Permissions</span></span>

<span data-ttu-id="7f599-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f599-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f599-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f599-110">Permission type</span></span>      | <span data-ttu-id="7f599-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f599-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f599-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f599-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f599-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f599-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7f599-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f599-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f599-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f599-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7f599-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f599-116">Application</span></span> | <span data-ttu-id="7f599-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f599-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f599-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f599-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="7f599-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f599-119">Request headers</span></span>

| <span data-ttu-id="7f599-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7f599-120">Name</span></span>       | <span data-ttu-id="7f599-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7f599-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f599-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f599-122">Authorization</span></span>  | <span data-ttu-id="7f599-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f599-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f599-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f599-125">Content-Type</span></span> | <span data-ttu-id="7f599-126">Строка, представляющая тип данных в теле сущности.</span><span class="sxs-lookup"><span data-stu-id="7f599-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="7f599-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f599-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f599-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f599-128">Request body</span></span>

<span data-ttu-id="7f599-129">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f599-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f599-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f599-130">Response</span></span>

<span data-ttu-id="7f599-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f599-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f599-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7f599-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f599-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f599-133">Request</span></span>

<span data-ttu-id="7f599-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f599-134">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f599-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f599-135">Response</span></span>

<span data-ttu-id="7f599-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f599-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->