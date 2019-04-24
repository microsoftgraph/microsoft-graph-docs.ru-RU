---
title: Получение объекта directoryRole
description: Получение свойств объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1194d982fdad6d73618b351395320b64d9400b96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454920"
---
# <a name="get-directoryrole"></a><span data-ttu-id="3a303-103">Получение объекта directoryRole</span><span class="sxs-lookup"><span data-stu-id="3a303-103">Get directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a303-104">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="3a303-104">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a303-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a303-105">Permissions</span></span>
<span data-ttu-id="3a303-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a303-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a303-108">Permission type</span></span>      | <span data-ttu-id="3a303-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a303-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a303-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a303-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a303-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a303-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a303-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a303-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a303-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a303-113">Not supported.</span></span>    |
|<span data-ttu-id="3a303-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a303-114">Application</span></span> | <span data-ttu-id="3a303-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a303-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a303-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a303-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a303-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a303-117">Optional query parameters</span></span>
<span data-ttu-id="3a303-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="3a303-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a303-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a303-119">Request headers</span></span>
| <span data-ttu-id="3a303-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a303-120">Name</span></span>       | <span data-ttu-id="3a303-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3a303-121">Type</span></span> | <span data-ttu-id="3a303-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a303-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a303-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a303-123">Authorization</span></span>  | <span data-ttu-id="3a303-124">string</span><span class="sxs-lookup"><span data-stu-id="3a303-124">string</span></span>  | <span data-ttu-id="3a303-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a303-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a303-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a303-127">Request body</span></span>
<span data-ttu-id="3a303-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a303-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a303-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a303-129">Response</span></span>

<span data-ttu-id="3a303-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a303-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a303-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a303-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a303-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a303-132">Request</span></span>
<span data-ttu-id="3a303-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a303-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="3a303-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a303-134">Response</span></span>
<span data-ttu-id="3a303-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a303-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
