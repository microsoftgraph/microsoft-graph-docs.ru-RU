---
title: Получение Импортедаппледевицеидентитиресулт
description: Чтение свойств и связей объекта Импортедаппледевицеидентитиресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56a85782e92c21dadb822b2f83e91e74074b79b9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981967"
---
# <a name="get-importedappledeviceidentityresult"></a><span data-ttu-id="4aac1-103">Получение Импортедаппледевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="4aac1-103">Get importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="4aac1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4aac1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4aac1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4aac1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aac1-106">Чтение свойств и связей объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="4aac1-106">Read properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4aac1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4aac1-107">Prerequisites</span></span>
<span data-ttu-id="4aac1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aac1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4aac1-110">Permission type</span></span>|<span data-ttu-id="4aac1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4aac1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4aac1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4aac1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4aac1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aac1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4aac1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4aac1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aac1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4aac1-115">Not supported.</span></span>|
|<span data-ttu-id="4aac1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4aac1-116">Application</span></span>|<span data-ttu-id="4aac1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4aac1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aac1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4aac1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4aac1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4aac1-119">Optional query parameters</span></span>
<span data-ttu-id="4aac1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4aac1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aac1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4aac1-121">Request headers</span></span>
|<span data-ttu-id="4aac1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4aac1-122">Header</span></span>|<span data-ttu-id="4aac1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4aac1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4aac1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4aac1-124">Authorization</span></span>|<span data-ttu-id="4aac1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4aac1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4aac1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4aac1-126">Accept</span></span>|<span data-ttu-id="4aac1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4aac1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aac1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4aac1-128">Request body</span></span>
<span data-ttu-id="4aac1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4aac1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aac1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4aac1-130">Response</span></span>
<span data-ttu-id="4aac1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4aac1-131">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aac1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4aac1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aac1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4aac1-133">Request</span></span>
<span data-ttu-id="4aac1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4aac1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="4aac1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aac1-135">Response</span></span>
<span data-ttu-id="4aac1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4aac1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
    "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
    "serialNumber": "Serial Number value",
    "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
    "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
    "isSupervised": true,
    "discoverySource": "adminImport",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "description": "Description value",
    "enrollmentState": "enrolled",
    "platform": "ios",
    "status": true
  }
}
```





