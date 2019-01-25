---
title: Создание synchronizationTemplate
description: Создание нового шаблона синхронизации для указанного приложения.
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509891"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="d9874-103">Создание synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="d9874-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9874-104">Создание нового шаблона синхронизации для указанного приложения.</span><span class="sxs-lookup"><span data-stu-id="d9874-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9874-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9874-105">Permissions</span></span>
<span data-ttu-id="d9874-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9874-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9874-108">Permission type</span></span>                        | <span data-ttu-id="d9874-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9874-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9874-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9874-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="d9874-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9874-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d9874-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9874-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d9874-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9874-113">Not supported.</span></span>|
|<span data-ttu-id="d9874-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9874-114">Application</span></span>                            |<span data-ttu-id="d9874-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9874-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="d9874-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9874-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="d9874-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9874-117">Request headers</span></span>

| <span data-ttu-id="d9874-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9874-118">Name</span></span>           | <span data-ttu-id="d9874-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d9874-119">Type</span></span>    | <span data-ttu-id="d9874-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9874-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d9874-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9874-121">Authorization</span></span>  | <span data-ttu-id="d9874-122">string</span><span class="sxs-lookup"><span data-stu-id="d9874-122">string</span></span>  | <span data-ttu-id="d9874-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9874-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9874-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9874-125">Request body</span></span>

<span data-ttu-id="d9874-126">В тексте запроса укажите создать объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="d9874-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="d9874-127">`id`, `applicationId` И `factoryTag` свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="d9874-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="d9874-128">Если нет `schema` предоставляется с помощью шаблона по умолчанию схема, связанная с `factoryTag` свойство будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="d9874-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="d9874-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9874-129">Response</span></span>

<span data-ttu-id="d9874-130">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d9874-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="d9874-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d9874-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9874-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9874-132">Request</span></span>
<span data-ttu-id="d9874-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9874-133">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d9874-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9874-134">Response</span></span>
<span data-ttu-id="d9874-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9874-135">The following is an example of a response.</span></span>
><span data-ttu-id="d9874-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d9874-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9874-137">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="d9874-137">All the properties will be returned in an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
