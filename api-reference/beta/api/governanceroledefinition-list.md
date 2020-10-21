---
title: Список Говернанцероледефинитионс
description: Получение коллекции Говернанцероледефинитионс для ресурса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5886be0267d0fb476d4cc896878c83edad41db39
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634832"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="711af-103">Список Говернанцероледефинитионс</span><span class="sxs-lookup"><span data-stu-id="711af-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="711af-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="711af-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="711af-105">Получение коллекции [говернанцероледефинитионс](../resources/governanceroledefinition.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="711af-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="711af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-106">Permissions</span></span>
<span data-ttu-id="711af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="711af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="711af-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="711af-109">Azure resources</span></span>

| <span data-ttu-id="711af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-110">Permission type</span></span> | <span data-ttu-id="711af-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="711af-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="711af-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="711af-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="711af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711af-115">Not supported.</span></span> |
| <span data-ttu-id="711af-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="711af-116">Application</span></span> | <span data-ttu-id="711af-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="711af-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="711af-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="711af-118">Azure AD</span></span>

| <span data-ttu-id="711af-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-119">Permission type</span></span> | <span data-ttu-id="711af-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="711af-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711af-121">Delegated (work or school account)</span></span> | <span data-ttu-id="711af-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="711af-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="711af-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711af-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711af-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711af-124">Not supported.</span></span> |
| <span data-ttu-id="711af-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="711af-125">Application</span></span> | <span data-ttu-id="711af-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="711af-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="711af-127">Группы</span><span class="sxs-lookup"><span data-stu-id="711af-127">Groups</span></span>

|<span data-ttu-id="711af-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-128">Permission type</span></span> | <span data-ttu-id="711af-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711af-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="711af-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711af-130">Delegated (work or school account)</span></span> | <span data-ttu-id="711af-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="711af-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="711af-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711af-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711af-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711af-133">Not supported.</span></span> |
| <span data-ttu-id="711af-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="711af-134">Application</span></span> | <span data-ttu-id="711af-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="711af-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="711af-136">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="711af-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="711af-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="711af-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="711af-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="711af-138">Optional query parameters</span></span>
<span data-ttu-id="711af-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="711af-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="711af-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="711af-140">Request headers</span></span>
| <span data-ttu-id="711af-141">Имя</span><span class="sxs-lookup"><span data-stu-id="711af-141">Name</span></span>      |<span data-ttu-id="711af-142">Описание</span><span class="sxs-lookup"><span data-stu-id="711af-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="711af-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="711af-143">Authorization</span></span>  | <span data-ttu-id="711af-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="711af-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="711af-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="711af-145">Request body</span></span>
<span data-ttu-id="711af-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="711af-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="711af-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="711af-147">Response</span></span>
<span data-ttu-id="711af-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [говернанцероледефинитион](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="711af-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="711af-149">Пример</span><span class="sxs-lookup"><span data-stu-id="711af-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="711af-150">В этом примере показано, как получить все определения ролей для группы "компания" Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="711af-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="711af-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="711af-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="711af-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="711af-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


