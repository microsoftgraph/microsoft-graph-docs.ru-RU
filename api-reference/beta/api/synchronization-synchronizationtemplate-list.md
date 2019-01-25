---
title: Список существующих шаблонов синхронизации
description: Список шаблонов синхронизации, связанных с указанного приложения или участников-служб.
localization_priority: Normal
ms.openlocfilehash: 309d1ddd6d702652b14e10895de10486a5d23783
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523633"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="5abf1-103">Список существующих шаблонов синхронизации</span><span class="sxs-lookup"><span data-stu-id="5abf1-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5abf1-104">Список шаблонов синхронизации, связанных с указанного приложения или участников-служб.</span><span class="sxs-lookup"><span data-stu-id="5abf1-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="5abf1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5abf1-105">Permissions</span></span>
<span data-ttu-id="5abf1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5abf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5abf1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5abf1-108">Permission type</span></span>                        | <span data-ttu-id="5abf1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5abf1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5abf1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5abf1-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="5abf1-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5abf1-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5abf1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5abf1-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5abf1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5abf1-113">Not supported.</span></span>|
|<span data-ttu-id="5abf1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5abf1-114">Application</span></span>                            |<span data-ttu-id="5abf1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5abf1-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="5abf1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5abf1-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="5abf1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5abf1-117">Request headers</span></span>

| <span data-ttu-id="5abf1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5abf1-118">Name</span></span>           | <span data-ttu-id="5abf1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5abf1-119">Type</span></span>    | <span data-ttu-id="5abf1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5abf1-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5abf1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5abf1-121">Authorization</span></span>  | <span data-ttu-id="5abf1-122">string</span><span class="sxs-lookup"><span data-stu-id="5abf1-122">string</span></span>  | <span data-ttu-id="5abf1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5abf1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5abf1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5abf1-125">Request body</span></span>

<span data-ttu-id="5abf1-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5abf1-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="5abf1-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5abf1-127">Response</span></span>

<span data-ttu-id="5abf1-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и acollection [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) объектов в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5abf1-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="5abf1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5abf1-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5abf1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5abf1-130">Request</span></span>
<span data-ttu-id="5abf1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5abf1-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="5abf1-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5abf1-132">Response</span></span>
<span data-ttu-id="5abf1-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5abf1-133">The following is an example of a response.</span></span>
><span data-ttu-id="5abf1-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5abf1-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5abf1-135">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="5abf1-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
