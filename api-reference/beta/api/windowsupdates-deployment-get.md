---
title: Развертывание
description: Ознакомьтесь с свойствами и отношениями объекта развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 43081598030efc8ac4b3e30fe35d99931dde5d8f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068043"
---
# <a name="get-deployment"></a><span data-ttu-id="3c3d5-103">Развертывание</span><span class="sxs-lookup"><span data-stu-id="3c3d5-103">Get deployment</span></span>
<span data-ttu-id="3c3d5-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3c3d5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c3d5-105">Ознакомьтесь с свойствами и отношениями объекта [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="3c3d5-105">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c3d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c3d5-106">Permissions</span></span>
<span data-ttu-id="3c3d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c3d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c3d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c3d5-109">Permission type</span></span>|<span data-ttu-id="3c3d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c3d5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c3d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c3d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c3d5-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3d5-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="3c3d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c3d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c3d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c3d5-114">Not supported.</span></span>|
|<span data-ttu-id="3c3d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c3d5-115">Application</span></span>|<span data-ttu-id="3c3d5-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3d5-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c3d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c3d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c3d5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c3d5-118">Optional query parameters</span></span>
<span data-ttu-id="3c3d5-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3c3d5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c3d5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c3d5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c3d5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c3d5-121">Request headers</span></span>
|<span data-ttu-id="3c3d5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3c3d5-122">Name</span></span>|<span data-ttu-id="3c3d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3c3d5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c3d5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c3d5-124">Authorization</span></span>|<span data-ttu-id="3c3d5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c3d5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c3d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c3d5-127">Request body</span></span>
<span data-ttu-id="3c3d5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c3d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c3d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c3d5-129">Response</span></span>

<span data-ttu-id="3c3d5-130">В случае успешного применения этот метод возвращает код ответа и `200 OK` объект [развертывания](../resources/windowsupdates-deployment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c3d5-130">If successful, this method returns a `200 OK` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c3d5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c3d5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c3d5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c3d5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
```


### <a name="response"></a><span data-ttu-id="3c3d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c3d5-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

