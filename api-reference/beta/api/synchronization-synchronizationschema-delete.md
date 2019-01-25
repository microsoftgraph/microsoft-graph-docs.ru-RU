---
title: Удаление synchronizationSchema
description: Удаление настраиваемой схемы и сбрасывает схемы в конфигурации по умолчанию. Если схема удаляется в контексте шаблона, он возвращает схему одно связанное с помощью шаблона по умолчанию `factoryTag`.
localization_priority: Normal
ms.openlocfilehash: cb4c6295fe962ea9570da19b9b6ee8190b2024f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526993"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="38f52-104">Удаление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="38f52-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38f52-105">Удаление настраиваемой схемы и сбрасывает схемы в конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="38f52-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="38f52-106">Если схема удаляется в контексте шаблона, он возвращает схему одно связанное с помощью шаблона по умолчанию `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="38f52-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="38f52-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38f52-107">Permissions</span></span>
<span data-ttu-id="38f52-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38f52-110">Permission type</span></span>                        | <span data-ttu-id="38f52-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38f52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38f52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38f52-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="38f52-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f52-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="38f52-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38f52-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="38f52-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f52-115">Not supported.</span></span>|
|<span data-ttu-id="38f52-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38f52-116">Application</span></span>                            |<span data-ttu-id="38f52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f52-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="38f52-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38f52-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="38f52-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38f52-119">Request headers</span></span>

| <span data-ttu-id="38f52-120">Имя</span><span class="sxs-lookup"><span data-stu-id="38f52-120">Name</span></span>           | <span data-ttu-id="38f52-121">Тип</span><span class="sxs-lookup"><span data-stu-id="38f52-121">Type</span></span>    | <span data-ttu-id="38f52-122">Описание</span><span class="sxs-lookup"><span data-stu-id="38f52-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="38f52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f52-123">Authorization</span></span>  | <span data-ttu-id="38f52-124">string</span><span class="sxs-lookup"><span data-stu-id="38f52-124">string</span></span>  | <span data-ttu-id="38f52-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38f52-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38f52-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38f52-127">Request body</span></span>

<span data-ttu-id="38f52-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38f52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38f52-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="38f52-129">Response</span></span>

<span data-ttu-id="38f52-130">В случае успешного выполнения этот метод возвращает код отклика `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="38f52-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="38f52-131">Он не возвращает все действия в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38f52-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f52-132">Пример</span><span class="sxs-lookup"><span data-stu-id="38f52-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38f52-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="38f52-133">Request</span></span>
<span data-ttu-id="38f52-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38f52-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="38f52-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="38f52-135">Response</span></span>
<span data-ttu-id="38f52-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="38f52-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
