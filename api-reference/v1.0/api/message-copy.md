---
title: 'message: copy'
description: Копирование сообщения в папку.
ms.openlocfilehash: 0883c847030eaf72f96a0ca4665bf002feba8ca2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028425"
---
# <a name="message-copy"></a><span data-ttu-id="b7e42-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="b7e42-103">message: copy</span></span>

<span data-ttu-id="b7e42-104">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="b7e42-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7e42-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e42-105">Permissions</span></span>

<span data-ttu-id="b7e42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7e42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7e42-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e42-108">Permission type</span></span> | <span data-ttu-id="b7e42-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7e42-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="b7e42-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7e42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7e42-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7e42-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7e42-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7e42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e42-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7e42-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7e42-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7e42-114">Application</span></span> | <span data-ttu-id="b7e42-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7e42-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e42-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7e42-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="b7e42-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7e42-117">Request headers</span></span>

| <span data-ttu-id="b7e42-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7e42-118">Header</span></span> | <span data-ttu-id="b7e42-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b7e42-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="b7e42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7e42-120">Authorization</span></span> | <span data-ttu-id="b7e42-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="b7e42-121"></span></span> <span data-ttu-id="b7e42-122">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="b7e42-122">Required.</span></span> |
| <span data-ttu-id="b7e42-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7e42-123">Content-Type</span></span> | <span data-ttu-id="b7e42-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="b7e42-124"></span></span> <span data-ttu-id="b7e42-125">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="b7e42-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7e42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7e42-126">Request body</span></span>

<span data-ttu-id="b7e42-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b7e42-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7e42-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="b7e42-128">Parameter</span></span> | <span data-ttu-id="b7e42-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b7e42-129">Type</span></span> | <span data-ttu-id="b7e42-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b7e42-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="b7e42-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="b7e42-131">destinationId</span></span>|<span data-ttu-id="b7e42-132">String</span><span class="sxs-lookup"><span data-stu-id="b7e42-132">String</span></span>|<span data-ttu-id="b7e42-133">Идентификатор папки назначения, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="b7e42-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="b7e42-134">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b7e42-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b7e42-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7e42-135">Response</span></span>

<span data-ttu-id="b7e42-136">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b7e42-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7e42-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b7e42-137">Example</span></span>

<span data-ttu-id="b7e42-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b7e42-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b7e42-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7e42-139">Request</span></span>
<span data-ttu-id="b7e42-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7e42-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="b7e42-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7e42-141">Response</span></span>

<span data-ttu-id="b7e42-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7e42-142">Here is an example of the response.</span></span>

> <span data-ttu-id="b7e42-143">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="b7e42-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7e42-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7e42-144">All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
