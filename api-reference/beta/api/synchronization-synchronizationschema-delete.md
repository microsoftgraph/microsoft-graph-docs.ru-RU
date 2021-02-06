---
title: Удаление synchronizationSchema
description: Удаляет настроенную схему и сбрасывает ее до конфигурации по умолчанию. Если схема удаляется в контексте шаблона, она сбрасывает схему до схемы по умолчанию, связанной с `factoryTag` шаблоном.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: f0ad4c43baa707d6ad6a4a35aa5919c45c2208be
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137370"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="b6cca-104">Удаление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="b6cca-104">Delete synchronizationSchema</span></span>

<span data-ttu-id="b6cca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6cca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6cca-106">Удаляет настроенную схему и сбрасывает ее до конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6cca-106">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="b6cca-107">Если схема удаляется в контексте шаблона, она сбрасывает схему до схемы по умолчанию, связанной с `factoryTag` шаблоном.</span><span class="sxs-lookup"><span data-stu-id="b6cca-107">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6cca-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6cca-108">Permissions</span></span>
<span data-ttu-id="b6cca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6cca-111">Permission type</span></span>                        | <span data-ttu-id="b6cca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6cca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6cca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6cca-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="b6cca-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cca-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b6cca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6cca-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b6cca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6cca-116">Not supported.</span></span>|
|<span data-ttu-id="b6cca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6cca-117">Application</span></span>                            |<span data-ttu-id="b6cca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6cca-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b6cca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6cca-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="b6cca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6cca-120">Request headers</span></span>

| <span data-ttu-id="b6cca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b6cca-121">Name</span></span>           | <span data-ttu-id="b6cca-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b6cca-122">Type</span></span>    | <span data-ttu-id="b6cca-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b6cca-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b6cca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6cca-124">Authorization</span></span>  | <span data-ttu-id="b6cca-125">string</span><span class="sxs-lookup"><span data-stu-id="b6cca-125">string</span></span>  | <span data-ttu-id="b6cca-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6cca-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6cca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6cca-128">Request body</span></span>

<span data-ttu-id="b6cca-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6cca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6cca-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6cca-130">Response</span></span>

<span data-ttu-id="b6cca-131">В случае успешного выполнения этот метод возвращает код отклика `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6cca-131">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="b6cca-132">Он не возвращает ничего в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b6cca-132">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6cca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b6cca-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b6cca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6cca-134">Request</span></span>
<span data-ttu-id="b6cca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6cca-135">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="b6cca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6cca-136">Response</span></span>
<span data-ttu-id="b6cca-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6cca-137">The following is an example of a response.</span></span>
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
  "suppressions": []
}
-->


