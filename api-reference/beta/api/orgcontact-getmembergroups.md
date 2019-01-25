---
title: 'orgContact: getMemberGroups'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 351db841ce8ca2cca5b2b3f29ca49f24fb281f04
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510136"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="62431-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="62431-104">orgContact: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="62431-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62431-105">Permissions</span></span>
<span data-ttu-id="62431-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62431-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62431-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62431-108">Permission type</span></span>      | <span data-ttu-id="62431-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62431-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62431-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62431-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62431-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62431-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62431-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62431-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62431-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62431-113">Not supported.</span></span>    |
|<span data-ttu-id="62431-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62431-114">Application</span></span> | <span data-ttu-id="62431-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62431-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62431-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62431-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="62431-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62431-117">Request headers</span></span>
| <span data-ttu-id="62431-118">Имя</span><span class="sxs-lookup"><span data-stu-id="62431-118">Name</span></span>       | <span data-ttu-id="62431-119">Тип</span><span class="sxs-lookup"><span data-stu-id="62431-119">Type</span></span> | <span data-ttu-id="62431-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62431-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62431-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62431-121">Authorization</span></span>  | <span data-ttu-id="62431-122">string</span><span class="sxs-lookup"><span data-stu-id="62431-122">string</span></span>  | <span data-ttu-id="62431-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62431-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62431-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62431-125">Request body</span></span>
<span data-ttu-id="62431-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="62431-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62431-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="62431-127">Parameter</span></span>    | <span data-ttu-id="62431-128">Тип</span><span class="sxs-lookup"><span data-stu-id="62431-128">Type</span></span>   |<span data-ttu-id="62431-129">Описание</span><span class="sxs-lookup"><span data-stu-id="62431-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62431-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="62431-130">securityEnabledOnly</span></span>|<span data-ttu-id="62431-131">Логическое</span><span class="sxs-lookup"><span data-stu-id="62431-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="62431-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="62431-132">Response</span></span>

<span data-ttu-id="62431-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62431-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62431-134">Пример</span><span class="sxs-lookup"><span data-stu-id="62431-134">Example</span></span>
<span data-ttu-id="62431-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="62431-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="62431-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="62431-136">Request</span></span>
<span data-ttu-id="62431-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62431-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="62431-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="62431-138">Response</span></span>
<span data-ttu-id="62431-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="62431-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
