---
title: Регистрация governanceResource
description: Регистрация объекта неуправляемые governanceResource в PIM.
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519047"
---
# <a name="register-governanceresource"></a><span data-ttu-id="0df33-103">Регистрация governanceResource</span><span class="sxs-lookup"><span data-stu-id="0df33-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df33-104">Регистрация объекта неуправляемые [governanceResource](../resources/governanceresource.md) в привилегированной управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="0df33-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df33-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0df33-105">Permissions</span></span>
<span data-ttu-id="0df33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0df33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="0df33-108">**Примечание:** Этот интерфейс API также требуется наличие по крайней мере один назначения роли active источник запроса на ресурс.</span><span class="sxs-lookup"><span data-stu-id="0df33-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="0df33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0df33-109">Permission type</span></span>      | <span data-ttu-id="0df33-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0df33-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0df33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0df33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0df33-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0df33-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0df33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0df33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0df33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0df33-114">Not supported.</span></span>    |
|<span data-ttu-id="0df33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0df33-115">Application</span></span> | <span data-ttu-id="0df33-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0df33-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="0df33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0df33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="0df33-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0df33-118">Optional query parameters</span></span>
<span data-ttu-id="0df33-119">Этот метод **только** поддерживает `$select` и `$expand` [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0df33-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="0df33-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0df33-120">Request headers</span></span>
| <span data-ttu-id="0df33-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0df33-121">Name</span></span>      |<span data-ttu-id="0df33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0df33-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0df33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0df33-123">Authorization</span></span>  | <span data-ttu-id="0df33-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0df33-124">Bearer {code}</span></span>|
| <span data-ttu-id="0df33-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0df33-125">Content-type</span></span>  | <span data-ttu-id="0df33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0df33-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="0df33-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0df33-127">Request body</span></span>

|<span data-ttu-id="0df33-128">Параметры</span><span class="sxs-lookup"><span data-stu-id="0df33-128">Parameters</span></span>      |<span data-ttu-id="0df33-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0df33-129">Type</span></span>                 |<span data-ttu-id="0df33-130">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0df33-130">Required</span></span> |<span data-ttu-id="0df33-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0df33-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="0df33-132">externalId</span><span class="sxs-lookup"><span data-stu-id="0df33-132">externalId</span></span>    |<span data-ttu-id="0df33-133">String</span><span class="sxs-lookup"><span data-stu-id="0df33-133">String</span></span>                 |<span data-ttu-id="0df33-134">✓</span><span class="sxs-lookup"><span data-stu-id="0df33-134">✓</span></span>        |<span data-ttu-id="0df33-135">ExternalId ресурс, который должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="0df33-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="0df33-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0df33-136">Response</span></span>
<span data-ttu-id="0df33-137">Успешно завершена, этот метод возвращает `200 OK` ответа.</span><span class="sxs-lookup"><span data-stu-id="0df33-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="0df33-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0df33-138">Example</span></span>
<span data-ttu-id="0df33-139">В этом примере показано, как зарегистрировать подписка на Azure Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="0df33-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="0df33-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0df33-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="0df33-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0df33-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
