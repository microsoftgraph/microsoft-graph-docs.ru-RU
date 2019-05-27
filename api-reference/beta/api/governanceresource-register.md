---
title: Регистрация governanceResource
description: Регистрация неуправляемого объекта governanceResource в PIM.
localization_priority: Normal
ms.openlocfilehash: 814ccd84d449f20882e1febbf0d48216ba3f5b89
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422460"
---
# <a name="register-governanceresource"></a><span data-ttu-id="5ac14-103">Регистрация governanceResource</span><span class="sxs-lookup"><span data-stu-id="5ac14-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ac14-104">Регистрация неуправляемого объекта [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="5ac14-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ac14-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ac14-105">Permissions</span></span>
<span data-ttu-id="5ac14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="5ac14-108">**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5ac14-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="5ac14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ac14-109">Permission type</span></span>      | <span data-ttu-id="5ac14-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ac14-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ac14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ac14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ac14-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="5ac14-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="5ac14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ac14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ac14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ac14-114">Not supported.</span></span>    |
|<span data-ttu-id="5ac14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ac14-115">Application</span></span> | <span data-ttu-id="5ac14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ac14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ac14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ac14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="5ac14-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ac14-118">Optional query parameters</span></span>
<span data-ttu-id="5ac14-119">Этот метод \*\*\*\* поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ac14-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="5ac14-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ac14-120">Request headers</span></span>
| <span data-ttu-id="5ac14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5ac14-121">Name</span></span>      |<span data-ttu-id="5ac14-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac14-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ac14-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ac14-123">Authorization</span></span>  | <span data-ttu-id="5ac14-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5ac14-124">Bearer {code}</span></span>|
| <span data-ttu-id="5ac14-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ac14-125">Content-type</span></span>  | <span data-ttu-id="5ac14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ac14-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="5ac14-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ac14-127">Request body</span></span>

|<span data-ttu-id="5ac14-128">Параметры</span><span class="sxs-lookup"><span data-stu-id="5ac14-128">Parameters</span></span>      |<span data-ttu-id="5ac14-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5ac14-129">Type</span></span>                 |<span data-ttu-id="5ac14-130">Обязательный</span><span class="sxs-lookup"><span data-stu-id="5ac14-130">Required</span></span> |<span data-ttu-id="5ac14-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac14-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="5ac14-132">externalId</span><span class="sxs-lookup"><span data-stu-id="5ac14-132">externalId</span></span>    |<span data-ttu-id="5ac14-133">String</span><span class="sxs-lookup"><span data-stu-id="5ac14-133">String</span></span>                 |<span data-ttu-id="5ac14-134">✓</span><span class="sxs-lookup"><span data-stu-id="5ac14-134">✓</span></span>        |<span data-ttu-id="5ac14-135">Екстерналид ресурса, регистрируемого в PIM.</span><span class="sxs-lookup"><span data-stu-id="5ac14-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="5ac14-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ac14-136">Response</span></span>
<span data-ttu-id="5ac14-137">В случае успешного выполнения этот метод возвращает `200 OK` отклик.</span><span class="sxs-lookup"><span data-stu-id="5ac14-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="5ac14-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5ac14-138">Example</span></span>
<span data-ttu-id="5ac14-139">В этом примере показано, как зарегистрировать подписку Azure Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="5ac14-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="5ac14-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ac14-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="5ac14-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ac14-141">Response</span></span>
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
  "suppressions": []
}
-->
