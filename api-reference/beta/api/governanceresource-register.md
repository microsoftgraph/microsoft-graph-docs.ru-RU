---
title: Регистрация governanceResource
description: Регистрация объекта неуправляемые governanceResource в PIM.
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837753"
---
# <a name="register-governanceresource"></a><span data-ttu-id="c13b0-103">Регистрация governanceResource</span><span class="sxs-lookup"><span data-stu-id="c13b0-103">Register governanceResource</span></span>

> <span data-ttu-id="c13b0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c13b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c13b0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c13b0-106">Регистрация объекта неуправляемые [governanceResource](../resources/governanceresource.md) в привилегированной управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="c13b0-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="c13b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c13b0-107">Permissions</span></span>
<span data-ttu-id="c13b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c13b0-110">**Примечание:** Этот интерфейс API также требуется наличие по крайней мере один назначения роли active источник запроса на ресурс.</span><span class="sxs-lookup"><span data-stu-id="c13b0-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="c13b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c13b0-111">Permission type</span></span>      | <span data-ttu-id="c13b0-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="c13b0-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c13b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c13b0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c13b0-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c13b0-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c13b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c13b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13b0-116">Not supported.</span></span>    |
|<span data-ttu-id="c13b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c13b0-117">Application</span></span> | <span data-ttu-id="c13b0-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c13b0-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="c13b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c13b0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="c13b0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c13b0-120">Optional query parameters</span></span>
<span data-ttu-id="c13b0-121">Этот метод **только** поддерживает `$select` и `$expand` [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c13b0-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="c13b0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c13b0-122">Request headers</span></span>
| <span data-ttu-id="c13b0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c13b0-123">Name</span></span>      |<span data-ttu-id="c13b0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c13b0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c13b0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c13b0-125">Authorization</span></span>  | <span data-ttu-id="c13b0-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c13b0-126">Bearer {code}</span></span>|
| <span data-ttu-id="c13b0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c13b0-127">Content-type</span></span>  | <span data-ttu-id="c13b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c13b0-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="c13b0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c13b0-129">Request body</span></span>

|<span data-ttu-id="c13b0-130">Параметры</span><span class="sxs-lookup"><span data-stu-id="c13b0-130">Parameters</span></span>      |<span data-ttu-id="c13b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c13b0-131">Type</span></span>                 |<span data-ttu-id="c13b0-132">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c13b0-132">Required</span></span> |<span data-ttu-id="c13b0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c13b0-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="c13b0-134">externalId</span><span class="sxs-lookup"><span data-stu-id="c13b0-134">externalId</span></span>    |<span data-ttu-id="c13b0-135">String</span><span class="sxs-lookup"><span data-stu-id="c13b0-135">String</span></span>                 |<span data-ttu-id="c13b0-136">✓</span><span class="sxs-lookup"><span data-stu-id="c13b0-136">✓</span></span>        |<span data-ttu-id="c13b0-137">ExternalId ресурс, который должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c13b0-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="c13b0-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="c13b0-138">Response</span></span>
<span data-ttu-id="c13b0-139">Успешно завершена, этот метод возвращает `200 OK` ответа.</span><span class="sxs-lookup"><span data-stu-id="c13b0-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="c13b0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c13b0-140">Example</span></span>
<span data-ttu-id="c13b0-141">В этом примере показано, как зарегистрировать подписка на Azure Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="c13b0-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="c13b0-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c13b0-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="c13b0-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="c13b0-143">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
