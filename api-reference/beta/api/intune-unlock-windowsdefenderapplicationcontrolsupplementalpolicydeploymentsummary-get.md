---
title: Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари
description: Чтение свойств и связей объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59491e6984e4bd2c430308590bbe4a8103ce9444
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087974"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="5cc93-103">Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари</span><span class="sxs-lookup"><span data-stu-id="5cc93-103">Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

> <span data-ttu-id="5cc93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc93-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cc93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc93-106">Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5cc93-106">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cc93-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5cc93-107">Prerequisites</span></span>
<span data-ttu-id="5cc93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cc93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cc93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cc93-110">Permission type</span></span>|<span data-ttu-id="5cc93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cc93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cc93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc93-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cc93-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5cc93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cc93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc93-115">Not supported.</span></span>|
|<span data-ttu-id="5cc93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cc93-116">Application</span></span>|<span data-ttu-id="5cc93-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cc93-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cc93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cc93-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cc93-119">Optional query parameters</span></span>
<span data-ttu-id="5cc93-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5cc93-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cc93-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cc93-121">Request headers</span></span>
|<span data-ttu-id="5cc93-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cc93-122">Header</span></span>|<span data-ttu-id="5cc93-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5cc93-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc93-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cc93-124">Authorization</span></span>|<span data-ttu-id="5cc93-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cc93-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cc93-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5cc93-126">Accept</span></span>|<span data-ttu-id="5cc93-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc93-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc93-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cc93-128">Request body</span></span>
<span data-ttu-id="5cc93-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cc93-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cc93-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cc93-130">Response</span></span>
<span data-ttu-id="5cc93-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cc93-131">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc93-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5cc93-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cc93-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cc93-133">Request</span></span>
<span data-ttu-id="5cc93-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cc93-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

### <a name="response"></a><span data-ttu-id="5cc93-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cc93-135">Response</span></span>
<span data-ttu-id="5cc93-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cc93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
    "id": "2f8656ed-56ed-2f86-ed56-862fed56862f",
    "deployedDeviceCount": 3,
    "failedDeviceCount": 1
  }
}
```






