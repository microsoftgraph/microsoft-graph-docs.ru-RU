---
title: Создание Синчронизатионтемплате
description: Создайте новый шаблон синхронизации для конкретного приложения.
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536966"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="463cc-103">Создание Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="463cc-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="463cc-104">Создайте новый шаблон синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="463cc-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="463cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="463cc-105">Permissions</span></span>
<span data-ttu-id="463cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="463cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="463cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="463cc-108">Permission type</span></span>                        | <span data-ttu-id="463cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="463cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="463cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="463cc-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="463cc-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="463cc-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="463cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="463cc-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="463cc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="463cc-113">Not supported.</span></span>|
|<span data-ttu-id="463cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="463cc-114">Application</span></span>                            |<span data-ttu-id="463cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="463cc-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="463cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="463cc-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="463cc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="463cc-117">Request headers</span></span>

| <span data-ttu-id="463cc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="463cc-118">Name</span></span>           | <span data-ttu-id="463cc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="463cc-119">Type</span></span>    | <span data-ttu-id="463cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="463cc-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="463cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="463cc-121">Authorization</span></span>  | <span data-ttu-id="463cc-122">string</span><span class="sxs-lookup"><span data-stu-id="463cc-122">string</span></span>  | <span data-ttu-id="463cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="463cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="463cc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="463cc-125">Request body</span></span>

<span data-ttu-id="463cc-126">В теле запроса добавьте объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) , который требуется создать.</span><span class="sxs-lookup"><span data-stu-id="463cc-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="463cc-127">`id`Свойства `applicationId` и `factoryTag` свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="463cc-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="463cc-128">Если с `schema` шаблоном не предоставляется никакой шаблон, будет использоваться схема по умолчанию, связанная со `factoryTag` свойством.</span><span class="sxs-lookup"><span data-stu-id="463cc-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="463cc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="463cc-129">Response</span></span>

<span data-ttu-id="463cc-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="463cc-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="463cc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="463cc-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="463cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="463cc-132">Request</span></span>
<span data-ttu-id="463cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="463cc-133">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="463cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="463cc-134">Response</span></span>
<span data-ttu-id="463cc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="463cc-135">The following is an example of a response.</span></span>
><span data-ttu-id="463cc-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="463cc-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="463cc-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="463cc-137">All the properties will be returned in an actual call.</span></span>
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
