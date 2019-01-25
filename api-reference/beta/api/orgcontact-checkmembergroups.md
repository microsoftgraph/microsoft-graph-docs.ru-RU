---
title: 'orgContact: checkMemberGroups'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9345a1879789a3f96a3eb6b2bbe4d636c75ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523787"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="7b089-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7b089-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="7b089-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b089-105">Permissions</span></span>
<span data-ttu-id="7b089-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b089-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b089-108">Permission type</span></span>      | <span data-ttu-id="7b089-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b089-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b089-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b089-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b089-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b089-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b089-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b089-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b089-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b089-113">Not supported.</span></span>    |
|<span data-ttu-id="7b089-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b089-114">Application</span></span> | <span data-ttu-id="7b089-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b089-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b089-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b089-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="7b089-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b089-117">Request headers</span></span>
| <span data-ttu-id="7b089-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7b089-118">Name</span></span>       | <span data-ttu-id="7b089-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7b089-119">Type</span></span> | <span data-ttu-id="7b089-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7b089-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b089-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b089-121">Authorization</span></span>  | <span data-ttu-id="7b089-122">string</span><span class="sxs-lookup"><span data-stu-id="7b089-122">string</span></span>  | <span data-ttu-id="7b089-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b089-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b089-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b089-125">Request body</span></span>
<span data-ttu-id="7b089-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7b089-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b089-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b089-127">Parameter</span></span>    | <span data-ttu-id="7b089-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7b089-128">Type</span></span>   |<span data-ttu-id="7b089-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7b089-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b089-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="7b089-130">groupIds</span></span>|<span data-ttu-id="7b089-131">String</span><span class="sxs-lookup"><span data-stu-id="7b089-131">String</span></span>||

## <a name="response"></a><span data-ttu-id="7b089-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b089-132">Response</span></span>

<span data-ttu-id="7b089-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b089-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b089-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7b089-134">Example</span></span>
<span data-ttu-id="7b089-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7b089-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b089-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b089-136">Request</span></span>
<span data-ttu-id="7b089-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b089-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="7b089-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b089-138">Response</span></span>
<span data-ttu-id="7b089-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7b089-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
