---
title: Получение governanceResource
description: Получение свойств и связей объекта governanceResource.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 58bfab0115fabc835d62bfa02f5da0a96b34a6f3
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635084"
---
# <a name="get-governanceresource"></a><span data-ttu-id="1687b-103">Получение governanceResource</span><span class="sxs-lookup"><span data-stu-id="1687b-103">Get governanceResource</span></span>

<span data-ttu-id="1687b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1687b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1687b-105">Получение свойств и связей объекта [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="1687b-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1687b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-106">Permissions</span></span>
<span data-ttu-id="1687b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="1687b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="1687b-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="1687b-109">Azure resources</span></span>

| <span data-ttu-id="1687b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-110">Permission type</span></span> | <span data-ttu-id="1687b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1687b-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1687b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1687b-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1687b-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="1687b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1687b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1687b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1687b-115">Not supported.</span></span> |
| <span data-ttu-id="1687b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1687b-116">Application</span></span> | <span data-ttu-id="1687b-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="1687b-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="1687b-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="1687b-118">Azure AD</span></span>

| <span data-ttu-id="1687b-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-119">Permission type</span></span> | <span data-ttu-id="1687b-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1687b-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1687b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1687b-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1687b-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="1687b-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1687b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1687b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1687b-124">Not supported.</span></span> |
| <span data-ttu-id="1687b-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="1687b-125">Application</span></span> | <span data-ttu-id="1687b-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="1687b-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="1687b-127">Группы</span><span class="sxs-lookup"><span data-stu-id="1687b-127">Groups</span></span>

|<span data-ttu-id="1687b-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-128">Permission type</span></span> | <span data-ttu-id="1687b-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1687b-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="1687b-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1687b-130">Delegated (work or school account)</span></span> | <span data-ttu-id="1687b-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="1687b-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="1687b-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1687b-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1687b-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1687b-133">Not supported.</span></span> |
| <span data-ttu-id="1687b-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="1687b-134">Application</span></span> | <span data-ttu-id="1687b-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="1687b-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="1687b-136">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="1687b-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="1687b-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1687b-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1687b-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1687b-138">Optional query parameters</span></span>
<span data-ttu-id="1687b-139">Этот метод **only** поддерживает только `$select` `$expand` [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1687b-139">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1687b-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1687b-140">Request headers</span></span>
| <span data-ttu-id="1687b-141">Имя</span><span class="sxs-lookup"><span data-stu-id="1687b-141">Name</span></span>      |<span data-ttu-id="1687b-142">Описание</span><span class="sxs-lookup"><span data-stu-id="1687b-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1687b-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1687b-143">Authorization</span></span>  | <span data-ttu-id="1687b-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1687b-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1687b-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1687b-145">Request body</span></span>
<span data-ttu-id="1687b-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1687b-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1687b-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="1687b-147">Response</span></span>
<span data-ttu-id="1687b-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1687b-148">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1687b-149">Пример</span><span class="sxs-lookup"><span data-stu-id="1687b-149">Example</span></span>
<span data-ttu-id="1687b-150">В этом примере показано, как получить сведения о подписке Wingtip Toys-произ (e5e7d29d-5465-45AC-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="1687b-150">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="1687b-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1687b-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="1687b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1687b-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


