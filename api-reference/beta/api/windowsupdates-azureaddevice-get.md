---
title: Get azureADDevice
description: Ознакомьтесь с свойствами объекта azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 22cf7a45e2782ee1a012e2ff1f02a94e9ff20401
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068200"
---
# <a name="get-azureaddevice"></a><span data-ttu-id="655bc-103">Get azureADDevice</span><span class="sxs-lookup"><span data-stu-id="655bc-103">Get azureADDevice</span></span>
<span data-ttu-id="655bc-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="655bc-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="655bc-105">Ознакомьтесь с свойствами объекта [azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="655bc-105">Read the properties of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="655bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="655bc-106">Permissions</span></span>
<span data-ttu-id="655bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="655bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="655bc-109">Permission type</span></span>|<span data-ttu-id="655bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="655bc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="655bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="655bc-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655bc-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="655bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="655bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="655bc-114">Not supported.</span></span>|
|<span data-ttu-id="655bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="655bc-115">Application</span></span>|<span data-ttu-id="655bc-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655bc-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="655bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="655bc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="655bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="655bc-118">Optional query parameters</span></span>
<span data-ttu-id="655bc-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="655bc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="655bc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="655bc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="655bc-121">Чтобы использовать параметр запроса для свойства, которое не наследуется [от updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="655bc-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="655bc-122">Например, чтобы выбрать свойство **ошибок,** используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="655bc-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="655bc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="655bc-123">Request headers</span></span>
|<span data-ttu-id="655bc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="655bc-124">Name</span></span>|<span data-ttu-id="655bc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="655bc-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="655bc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="655bc-126">Authorization</span></span>|<span data-ttu-id="655bc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="655bc-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="655bc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="655bc-129">Request body</span></span>
<span data-ttu-id="655bc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="655bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="655bc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="655bc-131">Response</span></span>

<span data-ttu-id="655bc-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект azureADDevice](../resources/windowsupdates-azureaddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="655bc-132">If successful, this method returns a `200 OK` response code and an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="655bc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="655bc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="655bc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="655bc-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a><span data-ttu-id="655bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="655bc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

