---
title: Создание synchronizationTemplate
description: Создание нового шаблона синхронизации для указанного приложения.
localization_priority: Normal
ms.openlocfilehash: 5b52c2ef180781faf8c93ce335d5f22ca8ae57cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822703"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="730ec-103">Создание synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="730ec-103">Create synchronizationTemplate</span></span>

> <span data-ttu-id="730ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="730ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="730ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="730ec-106">Создание нового шаблона синхронизации для указанного приложения.</span><span class="sxs-lookup"><span data-stu-id="730ec-106">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="730ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="730ec-107">Permissions</span></span>
<span data-ttu-id="730ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="730ec-110">Permission type</span></span>                        | <span data-ttu-id="730ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="730ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="730ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="730ec-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="730ec-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730ec-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="730ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="730ec-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="730ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730ec-115">Not supported.</span></span>|
|<span data-ttu-id="730ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="730ec-116">Application</span></span>                            |<span data-ttu-id="730ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730ec-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="730ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="730ec-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="730ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="730ec-119">Request headers</span></span>

| <span data-ttu-id="730ec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="730ec-120">Name</span></span>           | <span data-ttu-id="730ec-121">Тип</span><span class="sxs-lookup"><span data-stu-id="730ec-121">Type</span></span>    | <span data-ttu-id="730ec-122">Описание</span><span class="sxs-lookup"><span data-stu-id="730ec-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="730ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="730ec-123">Authorization</span></span>  | <span data-ttu-id="730ec-124">string</span><span class="sxs-lookup"><span data-stu-id="730ec-124">string</span></span>  | <span data-ttu-id="730ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="730ec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="730ec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="730ec-127">Request body</span></span>

<span data-ttu-id="730ec-128">В тексте запроса укажите создать объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="730ec-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="730ec-129">`id`, `applicationId` И `factoryTag` свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="730ec-129">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="730ec-130">Если нет `schema` предоставляется с помощью шаблона по умолчанию схема, связанная с `factoryTag` свойство будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="730ec-130">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="730ec-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="730ec-131">Response</span></span>

<span data-ttu-id="730ec-132">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="730ec-132">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="730ec-133">Пример</span><span class="sxs-lookup"><span data-stu-id="730ec-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="730ec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="730ec-134">Request</span></span>
<span data-ttu-id="730ec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="730ec-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="730ec-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="730ec-136">Response</span></span>
<span data-ttu-id="730ec-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="730ec-137">The following is an example of a response.</span></span>
><span data-ttu-id="730ec-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="730ec-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="730ec-139">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="730ec-139">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
