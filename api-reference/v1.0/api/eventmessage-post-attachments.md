---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 142de170aaf55a5c417be08a9fab4dafd7567ca3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584203"
---
# <a name="add-attachment"></a><span data-ttu-id="12527-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="12527-103">Add attachment</span></span>

<span data-ttu-id="12527-104">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="12527-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="12527-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="12527-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="12527-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="12527-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="12527-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="12527-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="12527-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="12527-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="12527-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="12527-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="12527-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12527-110">Permissions</span></span>
<span data-ttu-id="12527-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12527-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12527-113">Permission type</span></span>      | <span data-ttu-id="12527-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12527-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12527-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12527-115">Delegated (work or school account)</span></span> | <span data-ttu-id="12527-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12527-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="12527-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12527-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12527-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12527-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="12527-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12527-119">Application</span></span> | <span data-ttu-id="12527-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12527-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12527-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12527-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="12527-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12527-122">Request headers</span></span>
| <span data-ttu-id="12527-123">Имя</span><span class="sxs-lookup"><span data-stu-id="12527-123">Name</span></span>       | <span data-ttu-id="12527-124">Тип</span><span class="sxs-lookup"><span data-stu-id="12527-124">Type</span></span> | <span data-ttu-id="12527-125">Описание</span><span class="sxs-lookup"><span data-stu-id="12527-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12527-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="12527-126">Authorization</span></span>  | <span data-ttu-id="12527-127">string</span><span class="sxs-lookup"><span data-stu-id="12527-127">string</span></span>  | <span data-ttu-id="12527-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12527-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12527-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12527-130">Content-Type</span></span> | <span data-ttu-id="12527-131">string</span><span class="sxs-lookup"><span data-stu-id="12527-131">string</span></span>  | <span data-ttu-id="12527-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12527-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12527-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12527-134">Request body</span></span>
<span data-ttu-id="12527-135">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12527-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12527-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="12527-136">Response</span></span>

<span data-ttu-id="12527-137">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12527-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="12527-138">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="12527-138">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="12527-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="12527-139">Request</span></span>
<span data-ttu-id="12527-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12527-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="12527-141">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12527-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="12527-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="12527-142">Response</span></span>
<span data-ttu-id="12527-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12527-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="12527-146">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="12527-146">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="12527-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="12527-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="12527-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="12527-148">Response</span></span>
<span data-ttu-id="12527-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12527-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
