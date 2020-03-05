---
title: 'governanceResource: Register'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9edd34e7d8bd0fc2bd94f7d6afc0f038d8a250fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421349"
---
# <a name="governanceresource-register"></a><span data-ttu-id="b4ba5-103">governanceResource: Register</span><span class="sxs-lookup"><span data-stu-id="b4ba5-103">governanceResource: register</span></span>

<span data-ttu-id="b4ba5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b4ba5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ba5-105">Зарегистрируйте объект [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ba5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ba5-106">Permissions</span></span>

<span data-ttu-id="b4ba5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="b4ba5-109">**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="b4ba5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ba5-110">Permission type</span></span> | <span data-ttu-id="b4ba5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ba5-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b4ba5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4ba5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ba5-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b4ba5-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b4ba5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4ba5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ba5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-115">Not supported.</span></span> |
| <span data-ttu-id="b4ba5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4ba5-116">Application</span></span> | <span data-ttu-id="b4ba5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ba5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4ba5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4ba5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4ba5-119">Optional query parameters</span></span>

<span data-ttu-id="b4ba5-120">Этот метод \*\*\*\* поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-120">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4ba5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4ba5-121">Request headers</span></span>

| <span data-ttu-id="b4ba5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b4ba5-122">Name</span></span> | <span data-ttu-id="b4ba5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b4ba5-123">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="b4ba5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ba5-124">Authorization</span></span> | <span data-ttu-id="b4ba5-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b4ba5-125">Bearer {token}</span></span> |
| <span data-ttu-id="b4ba5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4ba5-126">Content-type</span></span> | <span data-ttu-id="b4ba5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b4ba5-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ba5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4ba5-128">Request body</span></span>

| <span data-ttu-id="b4ba5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4ba5-129">Properties</span></span> | <span data-ttu-id="b4ba5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4ba5-130">Type</span></span> | <span data-ttu-id="b4ba5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4ba5-131">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="b4ba5-132">externalId</span><span class="sxs-lookup"><span data-stu-id="b4ba5-132">externalId</span></span> | <span data-ttu-id="b4ba5-133">String</span><span class="sxs-lookup"><span data-stu-id="b4ba5-133">String</span></span> | <span data-ttu-id="b4ba5-134">Внешний идентификатор ресурса, регистрируемого в PIM.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-134">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="b4ba5-135">При регистрации подписки идентификатором является идентификатор подписки, добавленный в начале `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-135">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="b4ba5-136">Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-136">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="b4ba5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ba5-137">Response</span></span>

<span data-ttu-id="b4ba5-138">В случае успешного выполнения этот метод возвращает `200 OK` отклик.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-138">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="b4ba5-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b4ba5-139">Example</span></span>

<span data-ttu-id="b4ba5-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-140">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="b4ba5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4ba5-141">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="b4ba5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ba5-142">Response</span></span>
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
