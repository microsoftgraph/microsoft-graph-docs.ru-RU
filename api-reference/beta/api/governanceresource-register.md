---
title: 'governanceResource: Register'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fc6f2dd3ab6ba4cddc1ba3b3cde0e80ff268bb70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954279"
---
# <a name="governanceresource-register"></a><span data-ttu-id="c9efb-103">governanceResource: Register</span><span class="sxs-lookup"><span data-stu-id="c9efb-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9efb-104">Зарегистрируйте объект [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="c9efb-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9efb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9efb-105">Permissions</span></span>

<span data-ttu-id="c9efb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c9efb-108">**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c9efb-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="c9efb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9efb-109">Permission type</span></span> | <span data-ttu-id="c9efb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9efb-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c9efb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9efb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9efb-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="c9efb-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c9efb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9efb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9efb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9efb-114">Not supported.</span></span> |
| <span data-ttu-id="c9efb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9efb-115">Application</span></span> | <span data-ttu-id="c9efb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9efb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9efb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9efb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9efb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9efb-118">Optional query parameters</span></span>

<span data-ttu-id="c9efb-119">Этот метод \*\*\*\* поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9efb-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9efb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9efb-120">Request headers</span></span>

| <span data-ttu-id="c9efb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c9efb-121">Name</span></span> | <span data-ttu-id="c9efb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c9efb-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c9efb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9efb-123">Authorization</span></span> | <span data-ttu-id="c9efb-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c9efb-124">Bearer {token}</span></span> |
| <span data-ttu-id="c9efb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9efb-125">Content-type</span></span> | <span data-ttu-id="c9efb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9efb-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9efb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9efb-127">Request body</span></span>

| <span data-ttu-id="c9efb-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9efb-128">Properties</span></span> | <span data-ttu-id="c9efb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c9efb-129">Type</span></span> | <span data-ttu-id="c9efb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c9efb-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="c9efb-131">externalId</span><span class="sxs-lookup"><span data-stu-id="c9efb-131">externalId</span></span> | <span data-ttu-id="c9efb-132">String</span><span class="sxs-lookup"><span data-stu-id="c9efb-132">String</span></span> | <span data-ttu-id="c9efb-133">Внешний идентификатор ресурса, регистрируемого в PIM.</span><span class="sxs-lookup"><span data-stu-id="c9efb-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="c9efb-134">При регистрации подписки идентификатором является идентификатор подписки, добавленный в начале `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="c9efb-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="c9efb-135">Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="c9efb-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="c9efb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9efb-136">Response</span></span>

<span data-ttu-id="c9efb-137">В случае успешного выполнения этот метод возвращает `200 OK` отклик.</span><span class="sxs-lookup"><span data-stu-id="c9efb-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="c9efb-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c9efb-138">Example</span></span>

<span data-ttu-id="c9efb-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c9efb-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="c9efb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9efb-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="c9efb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9efb-141">Response</span></span>
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
