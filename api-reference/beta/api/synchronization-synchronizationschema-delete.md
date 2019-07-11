---
title: Удаление Синчронизатионсчема
description: Удаляет настраиваемую схему и восстанавливает конфигурацию схемы по умолчанию. Если схема удалена в контексте шаблона, она сбрасывается в схему по умолчанию, связанную с шаблоном `factoryTag`.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a4b3410f89e301205eee900fd1164b5c4445b103
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621034"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="58478-104">Удаление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="58478-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58478-105">Удаляет настраиваемую схему и восстанавливает конфигурацию схемы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58478-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="58478-106">Если схема удалена в контексте шаблона, она сбрасывается в схему по умолчанию, связанную с шаблоном `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="58478-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="58478-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58478-107">Permissions</span></span>
<span data-ttu-id="58478-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58478-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58478-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58478-110">Permission type</span></span>                        | <span data-ttu-id="58478-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58478-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="58478-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58478-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="58478-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58478-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="58478-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58478-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="58478-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58478-115">Not supported.</span></span>|
|<span data-ttu-id="58478-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58478-116">Application</span></span>                            |<span data-ttu-id="58478-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58478-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="58478-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58478-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="58478-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58478-119">Request headers</span></span>

| <span data-ttu-id="58478-120">Имя</span><span class="sxs-lookup"><span data-stu-id="58478-120">Name</span></span>           | <span data-ttu-id="58478-121">Тип</span><span class="sxs-lookup"><span data-stu-id="58478-121">Type</span></span>    | <span data-ttu-id="58478-122">Описание</span><span class="sxs-lookup"><span data-stu-id="58478-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="58478-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58478-123">Authorization</span></span>  | <span data-ttu-id="58478-124">string</span><span class="sxs-lookup"><span data-stu-id="58478-124">string</span></span>  | <span data-ttu-id="58478-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58478-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58478-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58478-127">Request body</span></span>

<span data-ttu-id="58478-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58478-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58478-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="58478-129">Response</span></span>

<span data-ttu-id="58478-130">В случае успешного выполнения этот метод возвращает код отклика `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="58478-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="58478-131">Он не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58478-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="58478-132">Пример</span><span class="sxs-lookup"><span data-stu-id="58478-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58478-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="58478-133">Request</span></span>
<span data-ttu-id="58478-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58478-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="58478-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="58478-135">Response</span></span>
<span data-ttu-id="58478-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58478-136">The following is an example of a response.</span></span>
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
