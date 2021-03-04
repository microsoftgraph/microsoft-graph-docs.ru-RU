---
title: 'governanceResource: регистрация'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: fed82587a1132b6c39e6e27e09546906792486b0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435947"
---
# <a name="governanceresource-register"></a><span data-ttu-id="a7015-103">governanceResource: регистрация</span><span class="sxs-lookup"><span data-stu-id="a7015-103">governanceResource: register</span></span>

<span data-ttu-id="a7015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7015-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7015-105">Регистрация объекта [governanceResource в](../resources/governanceresource.md) привилегированном управлении удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="a7015-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7015-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-106">Permissions</span></span>

<span data-ttu-id="a7015-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="a7015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="a7015-109">**Примечание:** Этот API также требует, чтобы у запрашиваемой стороны было по крайней мере одно назначение активной роли на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a7015-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="a7015-110">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="a7015-110">Azure resources</span></span>

| <span data-ttu-id="a7015-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-111">Permission type</span></span> | <span data-ttu-id="a7015-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a7015-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7015-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a7015-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a7015-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a7015-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7015-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7015-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-116">Not supported.</span></span> |
| <span data-ttu-id="a7015-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7015-117">Application</span></span> | <span data-ttu-id="a7015-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="a7015-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="a7015-119">Azure AD</span></span>

| <span data-ttu-id="a7015-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-120">Permission type</span></span> | <span data-ttu-id="a7015-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a7015-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7015-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a7015-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a7015-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="a7015-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7015-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7015-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-125">Not supported.</span></span> |
| <span data-ttu-id="a7015-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7015-126">Application</span></span> | <span data-ttu-id="a7015-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="a7015-128">Группы</span><span class="sxs-lookup"><span data-stu-id="a7015-128">Groups</span></span>

|<span data-ttu-id="a7015-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-129">Permission type</span></span> | <span data-ttu-id="a7015-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7015-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="a7015-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7015-131">Delegated (work or school account)</span></span> | <span data-ttu-id="a7015-132">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="a7015-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="a7015-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7015-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7015-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-134">Not supported.</span></span> |
| <span data-ttu-id="a7015-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7015-135">Application</span></span> | <span data-ttu-id="a7015-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7015-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7015-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7015-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7015-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7015-138">Optional query parameters</span></span>

<span data-ttu-id="a7015-139">Этот метод **поддерживает** только `$select` параметры `$expand` [запроса oData и OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="a7015-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7015-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7015-140">Request headers</span></span>

| <span data-ttu-id="a7015-141">Имя</span><span class="sxs-lookup"><span data-stu-id="a7015-141">Name</span></span> | <span data-ttu-id="a7015-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a7015-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a7015-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7015-143">Authorization</span></span> | <span data-ttu-id="a7015-144">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a7015-144">Bearer {token}</span></span> |
| <span data-ttu-id="a7015-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7015-145">Content-type</span></span> | <span data-ttu-id="a7015-146">application/json</span><span class="sxs-lookup"><span data-stu-id="a7015-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7015-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7015-147">Request body</span></span>

| <span data-ttu-id="a7015-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7015-148">Properties</span></span> | <span data-ttu-id="a7015-149">Тип</span><span class="sxs-lookup"><span data-stu-id="a7015-149">Type</span></span> | <span data-ttu-id="a7015-150">Описание</span><span class="sxs-lookup"><span data-stu-id="a7015-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="a7015-151">externalId</span><span class="sxs-lookup"><span data-stu-id="a7015-151">externalId</span></span> | <span data-ttu-id="a7015-152">String</span><span class="sxs-lookup"><span data-stu-id="a7015-152">String</span></span> | <span data-ttu-id="a7015-153">Внешний идентификатор ресурса, который будет зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="a7015-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="a7015-154">При регистрации подписки идентификатором является идентификатор подписки, предварительно заранее задверяющий `/subscriptions/` .</span><span class="sxs-lookup"><span data-stu-id="a7015-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="a7015-155">Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="a7015-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="a7015-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7015-156">Response</span></span>

<span data-ttu-id="a7015-157">В случае успешной работы этот метод возвращает `200 OK` ответ.</span><span class="sxs-lookup"><span data-stu-id="a7015-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="a7015-158">Пример</span><span class="sxs-lookup"><span data-stu-id="a7015-158">Example</span></span>

<span data-ttu-id="a7015-159">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a7015-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="a7015-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7015-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="a7015-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7015-161">Response</span></span>
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


