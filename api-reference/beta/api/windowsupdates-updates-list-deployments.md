---
title: Развертывание списков
description: Получите список объектов развертывания и их свойств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: f0e1028be3e9f8c5c49ebae42022ae71eda0c583
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068028"
---
# <a name="list-deployments"></a><span data-ttu-id="fecca-103">Развертывание списков</span><span class="sxs-lookup"><span data-stu-id="fecca-103">List deployments</span></span>
<span data-ttu-id="fecca-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fecca-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fecca-105">Получите список объектов [развертывания](../resources/windowsupdates-deployment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="fecca-105">Get a list of [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fecca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fecca-106">Permissions</span></span>
<span data-ttu-id="fecca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fecca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fecca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fecca-109">Permission type</span></span>|<span data-ttu-id="fecca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fecca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fecca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fecca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fecca-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecca-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="fecca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fecca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fecca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fecca-114">Not supported.</span></span>|
|<span data-ttu-id="fecca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fecca-115">Application</span></span>|<span data-ttu-id="fecca-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecca-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fecca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fecca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fecca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fecca-118">Optional query parameters</span></span>
<span data-ttu-id="fecca-119">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="fecca-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fecca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fecca-120">Request headers</span></span>
|<span data-ttu-id="fecca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fecca-121">Name</span></span>|<span data-ttu-id="fecca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fecca-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fecca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fecca-123">Authorization</span></span>|<span data-ttu-id="fecca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fecca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fecca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fecca-126">Request body</span></span>
<span data-ttu-id="fecca-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fecca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fecca-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fecca-128">Response</span></span>

<span data-ttu-id="fecca-129">В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` развертывания в тексте отклика. [](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="fecca-129">If successful, this method returns a `200 OK` response code and a collection of [deployment](../resources/windowsupdates-deployment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fecca-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="fecca-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fecca-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fecca-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments
```


### <a name="response"></a><span data-ttu-id="fecca-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fecca-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.deployment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
      "id": "b5171742-1742-b517-4217-17b5421717b5",
      "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
      },
      "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
      },
      "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

