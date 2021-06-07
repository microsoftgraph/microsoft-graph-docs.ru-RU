---
title: Получение объекта onPremisesConditionalAccessSettings
description: Чтение свойств и связей объекта onPremisesConditionalAccessSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db782f4d7e84455c2811480bb23e092370d719ff
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752513"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="bacec-103">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="bacec-103">Get onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="bacec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bacec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bacec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bacec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacec-106">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="bacec-106">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bacec-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bacec-107">Prerequisites</span></span>
<span data-ttu-id="bacec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bacec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bacec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bacec-110">Permission type</span></span>|<span data-ttu-id="bacec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bacec-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bacec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bacec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bacec-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacec-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bacec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bacec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bacec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacec-115">Not supported.</span></span>|
|<span data-ttu-id="bacec-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bacec-116">Application</span></span>|<span data-ttu-id="bacec-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacec-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bacec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bacec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bacec-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bacec-119">Optional query parameters</span></span>
<span data-ttu-id="bacec-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bacec-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bacec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bacec-121">Request headers</span></span>
|<span data-ttu-id="bacec-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bacec-122">Header</span></span>|<span data-ttu-id="bacec-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bacec-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bacec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bacec-124">Authorization</span></span>|<span data-ttu-id="bacec-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bacec-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bacec-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bacec-126">Accept</span></span>|<span data-ttu-id="bacec-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bacec-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bacec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bacec-128">Request body</span></span>
<span data-ttu-id="bacec-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bacec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bacec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacec-130">Response</span></span>
<span data-ttu-id="bacec-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bacec-131">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bacec-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bacec-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bacec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bacec-133">Request</span></span>
<span data-ttu-id="bacec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bacec-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="bacec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacec-135">Response</span></span>
<span data-ttu-id="bacec-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bacec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




