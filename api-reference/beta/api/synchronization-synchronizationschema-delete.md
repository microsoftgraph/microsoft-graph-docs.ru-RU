---
title: Удаление Синчронизатионсчема
description: Удаляет настраиваемую схему и восстанавливает конфигурацию схемы по умолчанию. Если схема удалена в контексте шаблона, она сбрасывается в схему по умолчанию, связанную с шаблоном `factoryTag`.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: affb05ba026be7c0ed4fbc4c09c09d1af8715ebc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452948"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="eae3f-104">Удаление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="eae3f-104">Delete synchronizationSchema</span></span>

<span data-ttu-id="eae3f-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eae3f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eae3f-106">Удаляет настраиваемую схему и восстанавливает конфигурацию схемы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eae3f-106">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="eae3f-107">Если схема удалена в контексте шаблона, она сбрасывается в схему по умолчанию, связанную с шаблоном `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="eae3f-107">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="eae3f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eae3f-108">Permissions</span></span>
<span data-ttu-id="eae3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eae3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eae3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eae3f-111">Permission type</span></span>                        | <span data-ttu-id="eae3f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eae3f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eae3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eae3f-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="eae3f-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eae3f-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="eae3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eae3f-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="eae3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae3f-116">Not supported.</span></span>|
|<span data-ttu-id="eae3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eae3f-117">Application</span></span>                            |<span data-ttu-id="eae3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae3f-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="eae3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eae3f-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="eae3f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eae3f-120">Request headers</span></span>

| <span data-ttu-id="eae3f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eae3f-121">Name</span></span>           | <span data-ttu-id="eae3f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="eae3f-122">Type</span></span>    | <span data-ttu-id="eae3f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eae3f-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="eae3f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eae3f-124">Authorization</span></span>  | <span data-ttu-id="eae3f-125">string</span><span class="sxs-lookup"><span data-stu-id="eae3f-125">string</span></span>  | <span data-ttu-id="eae3f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eae3f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eae3f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eae3f-128">Request body</span></span>

<span data-ttu-id="eae3f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eae3f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eae3f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eae3f-130">Response</span></span>

<span data-ttu-id="eae3f-131">В случае успешного выполнения этот метод возвращает код отклика `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eae3f-131">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="eae3f-132">Он не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eae3f-132">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="eae3f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="eae3f-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eae3f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="eae3f-134">Request</span></span>
<span data-ttu-id="eae3f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eae3f-135">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="eae3f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eae3f-136">Response</span></span>
<span data-ttu-id="eae3f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eae3f-137">The following is an example of a response.</span></span>
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
