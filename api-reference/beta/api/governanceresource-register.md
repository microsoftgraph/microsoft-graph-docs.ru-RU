---
title: 'governanceResource: регистрация'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 363ee47fcded93062b325f3f58df14dfa4a3c625
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350868"
---
# <a name="governanceresource-register"></a><span data-ttu-id="41485-103">governanceResource: регистрация</span><span class="sxs-lookup"><span data-stu-id="41485-103">governanceResource: register</span></span>

<span data-ttu-id="41485-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41485-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41485-105">Регистрация [объекта governanceResource](../resources/governanceresource.md) в управление привилегированными пользователями.</span><span class="sxs-lookup"><span data-stu-id="41485-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="41485-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-106">Permissions</span></span>

<span data-ttu-id="41485-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="41485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="41485-109">**Примечание:** Этот API также требует, чтобы у запрашиваемой стороны было по крайней мере одно назначение активной роли на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="41485-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="41485-110">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="41485-110">Azure resources</span></span>

| <span data-ttu-id="41485-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-111">Permission type</span></span> | <span data-ttu-id="41485-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="41485-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41485-113">Delegated (work or school account)</span></span> | <span data-ttu-id="41485-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="41485-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="41485-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41485-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41485-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-116">Not supported.</span></span> |
| <span data-ttu-id="41485-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41485-117">Application</span></span> | <span data-ttu-id="41485-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="41485-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="41485-119">Azure AD</span></span>

| <span data-ttu-id="41485-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-120">Permission type</span></span> | <span data-ttu-id="41485-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="41485-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41485-122">Delegated (work or school account)</span></span> | <span data-ttu-id="41485-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="41485-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="41485-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41485-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41485-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-125">Not supported.</span></span> |
| <span data-ttu-id="41485-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41485-126">Application</span></span> | <span data-ttu-id="41485-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="41485-128">Группы</span><span class="sxs-lookup"><span data-stu-id="41485-128">Groups</span></span>

|<span data-ttu-id="41485-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-129">Permission type</span></span> | <span data-ttu-id="41485-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41485-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="41485-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41485-131">Delegated (work or school account)</span></span> | <span data-ttu-id="41485-132">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="41485-132">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="41485-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41485-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41485-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-134">Not supported.</span></span> |
| <span data-ttu-id="41485-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41485-135">Application</span></span> | <span data-ttu-id="41485-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41485-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41485-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41485-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41485-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41485-138">Optional query parameters</span></span>

<span data-ttu-id="41485-139">Этот метод **поддерживает** только `$select` параметры `$expand` [запроса oData и OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="41485-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41485-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41485-140">Request headers</span></span>

| <span data-ttu-id="41485-141">Имя</span><span class="sxs-lookup"><span data-stu-id="41485-141">Name</span></span> | <span data-ttu-id="41485-142">Описание</span><span class="sxs-lookup"><span data-stu-id="41485-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="41485-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="41485-143">Authorization</span></span> | <span data-ttu-id="41485-144">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="41485-144">Bearer {token}</span></span> |
| <span data-ttu-id="41485-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41485-145">Content-type</span></span> | <span data-ttu-id="41485-146">application/json</span><span class="sxs-lookup"><span data-stu-id="41485-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="41485-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41485-147">Request body</span></span>

| <span data-ttu-id="41485-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="41485-148">Properties</span></span> | <span data-ttu-id="41485-149">Тип</span><span class="sxs-lookup"><span data-stu-id="41485-149">Type</span></span> | <span data-ttu-id="41485-150">Описание</span><span class="sxs-lookup"><span data-stu-id="41485-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="41485-151">externalId</span><span class="sxs-lookup"><span data-stu-id="41485-151">externalId</span></span> | <span data-ttu-id="41485-152">String</span><span class="sxs-lookup"><span data-stu-id="41485-152">String</span></span> | <span data-ttu-id="41485-153">Внешний идентификатор ресурса, который будет зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="41485-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="41485-154">При регистрации подписки идентификатором является идентификатор подписки, предварительно заранее задверяющий `/subscriptions/` .</span><span class="sxs-lookup"><span data-stu-id="41485-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="41485-155">Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="41485-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="41485-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="41485-156">Response</span></span>

<span data-ttu-id="41485-157">В случае успешной работы этот метод возвращает `200 OK` ответ.</span><span class="sxs-lookup"><span data-stu-id="41485-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="41485-158">Пример</span><span class="sxs-lookup"><span data-stu-id="41485-158">Example</span></span>

<span data-ttu-id="41485-159">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="41485-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="41485-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="41485-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="41485-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="41485-161">Response</span></span>
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


