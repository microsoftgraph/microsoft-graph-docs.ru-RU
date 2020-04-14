---
title: Функция Жетрелатедаппстатес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db38d8afa5c6be74bcc558c8cbdd7c141161c91d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441313"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="ef8b8-103">Функция Жетрелатедаппстатес</span><span class="sxs-lookup"><span data-stu-id="ef8b8-103">getRelatedAppStates function</span></span>

<span data-ttu-id="ef8b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef8b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef8b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef8b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef8b8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef8b8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef8b8-108">Prerequisites</span></span>
<span data-ttu-id="ef8b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef8b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef8b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef8b8-111">Permission type</span></span>|<span data-ttu-id="ef8b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef8b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef8b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef8b8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ef8b8-114">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="ef8b8-114">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="ef8b8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef8b8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ef8b8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef8b8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef8b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-117">Not supported.</span></span>|
|<span data-ttu-id="ef8b8-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef8b8-118">Application</span></span>||
| <span data-ttu-id="ef8b8-119">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="ef8b8-119">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="ef8b8-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef8b8-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef8b8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef8b8-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="ef8b8-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef8b8-122">Request headers</span></span>
|<span data-ttu-id="ef8b8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef8b8-123">Header</span></span>|<span data-ttu-id="ef8b8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ef8b8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef8b8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef8b8-125">Authorization</span></span>|<span data-ttu-id="ef8b8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef8b8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ef8b8-127">Accept</span></span>|<span data-ttu-id="ef8b8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ef8b8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef8b8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef8b8-129">Request body</span></span>
<span data-ttu-id="ef8b8-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ef8b8-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ef8b8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef8b8-132">Property</span></span>|<span data-ttu-id="ef8b8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ef8b8-133">Type</span></span>|<span data-ttu-id="ef8b8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ef8b8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef8b8-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef8b8-135">userPrincipalName</span></span>|<span data-ttu-id="ef8b8-136">String</span><span class="sxs-lookup"><span data-stu-id="ef8b8-136">String</span></span>|<span data-ttu-id="ef8b8-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-137">Not yet documented</span></span>|
|<span data-ttu-id="ef8b8-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="ef8b8-138">deviceId</span></span>|<span data-ttu-id="ef8b8-139">String</span><span class="sxs-lookup"><span data-stu-id="ef8b8-139">String</span></span>|<span data-ttu-id="ef8b8-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ef8b8-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ef8b8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef8b8-141">Response</span></span>
<span data-ttu-id="ef8b8-142">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [мобилеаппрелатионшипстате](../resources/intune-apps-mobileapprelationshipstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-142">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef8b8-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ef8b8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef8b8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef8b8-144">Request</span></span>
<span data-ttu-id="ef8b8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ef8b8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef8b8-146">Response</span></span>
<span data-ttu-id="ef8b8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef8b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






