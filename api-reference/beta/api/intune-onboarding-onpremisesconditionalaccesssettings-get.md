---
title: Получение объекта onPremisesConditionalAccessSettings
description: Чтение свойств и связей объекта onPremisesConditionalAccessSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39699f92108536369d5ca12d3f07e792f0d7b8ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156872"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="f4e20-103">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f4e20-103">Get onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="f4e20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4e20-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4e20-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4e20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e20-107">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f4e20-107">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4e20-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4e20-108">Prerequisites</span></span>
<span data-ttu-id="f4e20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e20-111">Permission type</span></span>|<span data-ttu-id="f4e20-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4e20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4e20-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4e20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4e20-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e20-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4e20-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4e20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4e20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e20-116">Not supported.</span></span>|
|<span data-ttu-id="f4e20-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4e20-117">Application</span></span>|<span data-ttu-id="f4e20-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e20-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4e20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4e20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4e20-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4e20-120">Optional query parameters</span></span>
<span data-ttu-id="f4e20-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f4e20-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4e20-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4e20-122">Request headers</span></span>
|<span data-ttu-id="f4e20-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4e20-123">Header</span></span>|<span data-ttu-id="f4e20-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f4e20-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4e20-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e20-125">Authorization</span></span>|<span data-ttu-id="f4e20-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4e20-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4e20-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f4e20-127">Accept</span></span>|<span data-ttu-id="f4e20-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f4e20-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4e20-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4e20-129">Request body</span></span>
<span data-ttu-id="f4e20-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4e20-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4e20-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e20-131">Response</span></span>
<span data-ttu-id="f4e20-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e20-132">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4e20-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f4e20-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4e20-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4e20-134">Request</span></span>
<span data-ttu-id="f4e20-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4e20-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="f4e20-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e20-136">Response</span></span>
<span data-ttu-id="f4e20-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4e20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




