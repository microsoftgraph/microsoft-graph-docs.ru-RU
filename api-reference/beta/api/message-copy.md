---
title: 'message: copy'
description: Копирование сообщения в папку.
ms.openlocfilehash: c0c5428ff2f661d865a6cb2cd17bc0a48e177a52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077054"
---
# <a name="message-copy"></a><span data-ttu-id="35922-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="35922-103">message: copy</span></span>

> <span data-ttu-id="35922-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35922-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35922-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35922-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35922-106">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="35922-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="35922-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35922-107">Permissions</span></span>

<span data-ttu-id="35922-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35922-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35922-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35922-110">Permission type</span></span> | <span data-ttu-id="35922-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35922-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="35922-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35922-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35922-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35922-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35922-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35922-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35922-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35922-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35922-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35922-116">Application</span></span> | <span data-ttu-id="35922-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35922-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35922-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35922-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="35922-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35922-119">Request headers</span></span>

| <span data-ttu-id="35922-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35922-120">Header</span></span> | <span data-ttu-id="35922-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35922-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="35922-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35922-122">Authorization</span></span> | <span data-ttu-id="35922-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="35922-123"></span></span> <span data-ttu-id="35922-124">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="35922-124">Required.</span></span> |
| <span data-ttu-id="35922-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35922-125">Content-Type</span></span> | <span data-ttu-id="35922-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="35922-126"></span></span> <span data-ttu-id="35922-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="35922-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35922-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35922-128">Request body</span></span>

<span data-ttu-id="35922-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="35922-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35922-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="35922-130">Parameter</span></span> | <span data-ttu-id="35922-131">Тип</span><span class="sxs-lookup"><span data-stu-id="35922-131">Type</span></span> | <span data-ttu-id="35922-132">Описание</span><span class="sxs-lookup"><span data-stu-id="35922-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="35922-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="35922-133">destinationId</span></span>|<span data-ttu-id="35922-134">String</span><span class="sxs-lookup"><span data-stu-id="35922-134">String</span></span>|<span data-ttu-id="35922-135">Идентификатор папки назначения, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="35922-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="35922-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="35922-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="35922-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="35922-137">Response</span></span>

<span data-ttu-id="35922-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="35922-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35922-139">Пример</span><span class="sxs-lookup"><span data-stu-id="35922-139">Example</span></span>

<span data-ttu-id="35922-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="35922-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="35922-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="35922-141">Request</span></span>

<span data-ttu-id="35922-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35922-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="35922-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="35922-143">Response</span></span>

<span data-ttu-id="35922-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35922-144">Here is an example of the response.</span></span>

> <span data-ttu-id="35922-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="35922-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="35922-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35922-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
