---
title: 'governanceResource: Register'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713921"
---
# <a name="governanceresource-register"></a><span data-ttu-id="211db-103">governanceResource: Register</span><span class="sxs-lookup"><span data-stu-id="211db-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="211db-104">Зарегистрируйте объект [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="211db-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="211db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="211db-105">Permissions</span></span>

<span data-ttu-id="211db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="211db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="211db-108">**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="211db-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="211db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="211db-109">Permission type</span></span> | <span data-ttu-id="211db-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="211db-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="211db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="211db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="211db-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="211db-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="211db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="211db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="211db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="211db-114">Not supported.</span></span> |
| <span data-ttu-id="211db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="211db-115">Application</span></span> | <span data-ttu-id="211db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="211db-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="211db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="211db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="211db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="211db-118">Optional query parameters</span></span>

<span data-ttu-id="211db-119">Этот метод \*\*\*\* поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="211db-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="211db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="211db-120">Request headers</span></span>

| <span data-ttu-id="211db-121">Имя</span><span class="sxs-lookup"><span data-stu-id="211db-121">Name</span></span> | <span data-ttu-id="211db-122">Описание</span><span class="sxs-lookup"><span data-stu-id="211db-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="211db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="211db-123">Authorization</span></span> | <span data-ttu-id="211db-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="211db-124">Bearer {token}</span></span> |
| <span data-ttu-id="211db-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="211db-125">Content-type</span></span> | <span data-ttu-id="211db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="211db-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="211db-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="211db-127">Request body</span></span>

| <span data-ttu-id="211db-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="211db-128">Properties</span></span> | <span data-ttu-id="211db-129">Тип</span><span class="sxs-lookup"><span data-stu-id="211db-129">Type</span></span> | <span data-ttu-id="211db-130">Описание</span><span class="sxs-lookup"><span data-stu-id="211db-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="211db-131">externalId</span><span class="sxs-lookup"><span data-stu-id="211db-131">externalId</span></span> | <span data-ttu-id="211db-132">String</span><span class="sxs-lookup"><span data-stu-id="211db-132">String</span></span> | <span data-ttu-id="211db-133">Внешний идентификатор ресурса, регистрируемого в PIM.</span><span class="sxs-lookup"><span data-stu-id="211db-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="211db-134">При регистрации подписки идентификатором является идентификатор подписки, добавленный в начале `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="211db-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="211db-135">Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="211db-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="211db-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="211db-136">Response</span></span>

<span data-ttu-id="211db-137">В случае успешного выполнения этот метод возвращает `200 OK` отклик.</span><span class="sxs-lookup"><span data-stu-id="211db-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="211db-138">Пример</span><span class="sxs-lookup"><span data-stu-id="211db-138">Example</span></span>

<span data-ttu-id="211db-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="211db-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="211db-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="211db-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="211db-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="211db-141">Response</span></span>
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
