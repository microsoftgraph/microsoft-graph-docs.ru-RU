---
title: Функция Жетрелатедаппстатес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15b3e278e669c17c6f66ae37976cd8c74ee702d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458296"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="f8cfd-103">Функция Жетрелатедаппстатес</span><span class="sxs-lookup"><span data-stu-id="f8cfd-103">getRelatedAppStates function</span></span>

<span data-ttu-id="f8cfd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8cfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8cfd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8cfd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8cfd-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8cfd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8cfd-108">Prerequisites</span></span>
<span data-ttu-id="f8cfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8cfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8cfd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8cfd-111">Permission type</span></span>|<span data-ttu-id="f8cfd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8cfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8cfd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8cfd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f8cfd-114">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="f8cfd-114">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="f8cfd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8cfd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8cfd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8cfd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8cfd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-117">Not supported.</span></span>|
|<span data-ttu-id="f8cfd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8cfd-118">Application</span></span>||
| <span data-ttu-id="f8cfd-119">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="f8cfd-119">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="f8cfd-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8cfd-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8cfd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8cfd-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="f8cfd-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8cfd-122">Request headers</span></span>
|<span data-ttu-id="f8cfd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8cfd-123">Header</span></span>|<span data-ttu-id="f8cfd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f8cfd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8cfd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8cfd-125">Authorization</span></span>|<span data-ttu-id="f8cfd-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8cfd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f8cfd-127">Accept</span></span>|<span data-ttu-id="f8cfd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f8cfd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8cfd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8cfd-129">Request body</span></span>
<span data-ttu-id="f8cfd-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f8cfd-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f8cfd-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8cfd-132">Property</span></span>|<span data-ttu-id="f8cfd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f8cfd-133">Type</span></span>|<span data-ttu-id="f8cfd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f8cfd-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8cfd-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8cfd-135">userPrincipalName</span></span>|<span data-ttu-id="f8cfd-136">String</span><span class="sxs-lookup"><span data-stu-id="f8cfd-136">String</span></span>|<span data-ttu-id="f8cfd-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-137">Not yet documented</span></span>|
|<span data-ttu-id="f8cfd-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="f8cfd-138">deviceId</span></span>|<span data-ttu-id="f8cfd-139">String</span><span class="sxs-lookup"><span data-stu-id="f8cfd-139">String</span></span>|<span data-ttu-id="f8cfd-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f8cfd-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f8cfd-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8cfd-141">Response</span></span>
<span data-ttu-id="f8cfd-142">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [мобилеаппрелатионшипстате](../resources/intune-apps-mobileapprelationshipstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-142">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8cfd-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f8cfd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8cfd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8cfd-144">Request</span></span>
<span data-ttu-id="f8cfd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f8cfd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8cfd-146">Response</span></span>
<span data-ttu-id="f8cfd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8cfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState",
      "sourceIds": [
        "Source Ids value"
      ],
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "deviceId": "Device Id value",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "targetLastSyncDateTime": "2017-01-01T00:02:09.7809949-08:00"
    }
  ]
}
```








