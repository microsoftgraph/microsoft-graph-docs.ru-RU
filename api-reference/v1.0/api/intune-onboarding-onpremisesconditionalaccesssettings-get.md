---
title: Получение объекта onPremisesConditionalAccessSettings
description: Чтение свойств и связей объекта onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97fbcbc1e0f9564495204525eb1db369acaa5d43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965280"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="03916-103">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="03916-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="03916-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03916-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03916-105">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="03916-105">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03916-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="03916-106">Prerequisites</span></span>
<span data-ttu-id="03916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03916-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03916-109">Permission type</span></span>|<span data-ttu-id="03916-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03916-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03916-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03916-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03916-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="03916-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="03916-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03916-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03916-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03916-114">Not supported.</span></span>|
|<span data-ttu-id="03916-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03916-115">Application</span></span>|<span data-ttu-id="03916-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03916-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03916-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03916-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03916-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03916-118">Optional query parameters</span></span>
<span data-ttu-id="03916-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03916-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="03916-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03916-120">Request headers</span></span>
|<span data-ttu-id="03916-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03916-121">Header</span></span>|<span data-ttu-id="03916-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03916-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03916-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03916-123">Authorization</span></span>|<span data-ttu-id="03916-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="03916-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03916-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03916-125">Accept</span></span>|<span data-ttu-id="03916-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03916-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03916-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03916-127">Request body</span></span>
<span data-ttu-id="03916-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03916-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03916-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03916-129">Response</span></span>
<span data-ttu-id="03916-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03916-130">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03916-131">Пример</span><span class="sxs-lookup"><span data-stu-id="03916-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="03916-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03916-132">Request</span></span>
<span data-ttu-id="03916-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03916-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="03916-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="03916-134">Response</span></span>
<span data-ttu-id="03916-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="03916-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```



