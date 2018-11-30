---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
ms.openlocfilehash: fdba426b8d461f94b676aac2da3af4996e6427c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075041"
---
# <a name="add-attachment"></a><span data-ttu-id="a2f0f-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="a2f0f-103">Add attachment</span></span>

> <span data-ttu-id="a2f0f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2f0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2f0f-106">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="a2f0f-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="a2f0f-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a2f0f-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a2f0f-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a2f0f-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a2f0f-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="a2f0f-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a2f0f-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="a2f0f-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a2f0f-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a2f0f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f0f-112">Permissions</span></span>
<span data-ttu-id="a2f0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2f0f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f0f-115">Permission type</span></span>      | <span data-ttu-id="a2f0f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2f0f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f0f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2f0f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f0f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2f0f-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2f0f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2f0f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f0f-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2f0f-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2f0f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2f0f-121">Application</span></span> | <span data-ttu-id="a2f0f-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2f0f-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2f0f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2f0f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="a2f0f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2f0f-124">Request headers</span></span>
| <span data-ttu-id="a2f0f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a2f0f-125">Name</span></span>       | <span data-ttu-id="a2f0f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a2f0f-126">Type</span></span> | <span data-ttu-id="a2f0f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a2f0f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2f0f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2f0f-128">Authorization</span></span>  | <span data-ttu-id="a2f0f-129">string</span><span class="sxs-lookup"><span data-stu-id="a2f0f-129">string</span></span>  | <span data-ttu-id="a2f0f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2f0f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2f0f-132">Content-Type</span></span> | <span data-ttu-id="a2f0f-133">string</span><span class="sxs-lookup"><span data-stu-id="a2f0f-133">string</span></span>  | <span data-ttu-id="a2f0f-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2f0f-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2f0f-136">Request body</span></span>
<span data-ttu-id="a2f0f-137">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a2f0f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2f0f-138">Response</span></span>

<span data-ttu-id="a2f0f-139">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a2f0f-140">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="a2f0f-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2f0f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2f0f-141">Request</span></span>
<span data-ttu-id="a2f0f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

##### <a name="response"></a><span data-ttu-id="a2f0f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2f0f-143">Response</span></span>
<span data-ttu-id="a2f0f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a2f0f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="a2f0f-147">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="a2f0f-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2f0f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2f0f-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="a2f0f-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2f0f-149">Response</span></span>
<span data-ttu-id="a2f0f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a2f0f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
