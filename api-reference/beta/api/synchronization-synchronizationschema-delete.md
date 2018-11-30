---
title: Удаление synchronizationSchema
description: Удаление настраиваемой схемы и сбрасывает схемы в конфигурации по умолчанию. Если схема удаляется в контексте шаблона, он возвращает схему одно связанное с помощью шаблона по умолчанию `factoryTag`.
ms.openlocfilehash: 81c1a918b10e8f4553b3e99312f20bb538bfbe4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080821"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="93a8a-104">Удаление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="93a8a-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="93a8a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93a8a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93a8a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a8a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93a8a-107">Удаление настраиваемой схемы и сбрасывает схемы в конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="93a8a-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="93a8a-108">Если схема удаляется в контексте шаблона, он возвращает схему одно связанное с помощью шаблона по умолчанию `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="93a8a-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="93a8a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93a8a-109">Permissions</span></span>
<span data-ttu-id="93a8a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93a8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93a8a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93a8a-112">Permission type</span></span>                        | <span data-ttu-id="93a8a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93a8a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93a8a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93a8a-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="93a8a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a8a-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="93a8a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93a8a-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="93a8a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a8a-117">Not supported.</span></span>|
|<span data-ttu-id="93a8a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93a8a-118">Application</span></span>                            |<span data-ttu-id="93a8a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a8a-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="93a8a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93a8a-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="93a8a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93a8a-121">Request headers</span></span>

| <span data-ttu-id="93a8a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="93a8a-122">Name</span></span>           | <span data-ttu-id="93a8a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="93a8a-123">Type</span></span>    | <span data-ttu-id="93a8a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="93a8a-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="93a8a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93a8a-125">Authorization</span></span>  | <span data-ttu-id="93a8a-126">string</span><span class="sxs-lookup"><span data-stu-id="93a8a-126">string</span></span>  | <span data-ttu-id="93a8a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93a8a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93a8a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93a8a-129">Request body</span></span>

<span data-ttu-id="93a8a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93a8a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93a8a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="93a8a-131">Response</span></span>

<span data-ttu-id="93a8a-132">В случае успешного выполнения этот метод возвращает код отклика `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93a8a-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="93a8a-133">Он не возвращает все действия в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="93a8a-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="93a8a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="93a8a-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93a8a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="93a8a-135">Request</span></span>
<span data-ttu-id="93a8a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93a8a-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="93a8a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="93a8a-137">Response</span></span>
<span data-ttu-id="93a8a-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93a8a-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->