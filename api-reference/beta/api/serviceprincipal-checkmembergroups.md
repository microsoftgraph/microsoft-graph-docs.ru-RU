---
title: 'servicePrincipal: Чеккмемберграупс'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
ms.openlocfilehash: 2237f83ce32bbb34f983226011f1c324185040b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545522"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="71b30-104">servicePrincipal: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="71b30-104">servicePrincipal: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="71b30-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71b30-105">Permissions</span></span>
<span data-ttu-id="71b30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b30-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b30-108">Permission type</span></span>      | <span data-ttu-id="71b30-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b30-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71b30-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71b30-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71b30-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b30-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b30-113">Not supported.</span></span>    |
|<span data-ttu-id="71b30-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b30-114">Application</span></span> | <span data-ttu-id="71b30-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="71b30-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b30-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="71b30-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b30-117">Request headers</span></span>
| <span data-ttu-id="71b30-118">Имя</span><span class="sxs-lookup"><span data-stu-id="71b30-118">Name</span></span>       | <span data-ttu-id="71b30-119">Тип</span><span class="sxs-lookup"><span data-stu-id="71b30-119">Type</span></span> | <span data-ttu-id="71b30-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71b30-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71b30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b30-121">Authorization</span></span>  | <span data-ttu-id="71b30-122">string</span><span class="sxs-lookup"><span data-stu-id="71b30-122">string</span></span>  | <span data-ttu-id="71b30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71b30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71b30-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71b30-125">Request body</span></span>
<span data-ttu-id="71b30-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="71b30-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71b30-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="71b30-127">Parameter</span></span>    | <span data-ttu-id="71b30-128">Тип</span><span class="sxs-lookup"><span data-stu-id="71b30-128">Type</span></span>   |<span data-ttu-id="71b30-129">Описание</span><span class="sxs-lookup"><span data-stu-id="71b30-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71b30-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="71b30-130">groupIds</span></span>|<span data-ttu-id="71b30-131">String</span><span class="sxs-lookup"><span data-stu-id="71b30-131">String</span></span>||

## <a name="response"></a><span data-ttu-id="71b30-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b30-132">Response</span></span>

<span data-ttu-id="71b30-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71b30-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b30-134">Пример</span><span class="sxs-lookup"><span data-stu-id="71b30-134">Example</span></span>
<span data-ttu-id="71b30-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="71b30-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71b30-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b30-136">Request</span></span>
<span data-ttu-id="71b30-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b30-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="71b30-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b30-138">Response</span></span>
<span data-ttu-id="71b30-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71b30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
