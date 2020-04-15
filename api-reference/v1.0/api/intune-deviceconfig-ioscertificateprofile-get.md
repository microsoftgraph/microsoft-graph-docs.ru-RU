---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e68a60bff6022a864eff4bb31f77cd25f3738ec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442113"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="476fd-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="476fd-103">Get iosCertificateProfile</span></span>

<span data-ttu-id="476fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="476fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="476fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="476fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="476fd-106">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="476fd-106">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="476fd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="476fd-107">Prerequisites</span></span>
<span data-ttu-id="476fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="476fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="476fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="476fd-110">Permission type</span></span>|<span data-ttu-id="476fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="476fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="476fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="476fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="476fd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="476fd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="476fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="476fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="476fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="476fd-115">Not supported.</span></span>|
|<span data-ttu-id="476fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="476fd-116">Application</span></span>|<span data-ttu-id="476fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="476fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="476fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="476fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="476fd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="476fd-119">Optional query parameters</span></span>
<span data-ttu-id="476fd-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="476fd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="476fd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="476fd-121">Request headers</span></span>
|<span data-ttu-id="476fd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="476fd-122">Header</span></span>|<span data-ttu-id="476fd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="476fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="476fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="476fd-124">Authorization</span></span>|<span data-ttu-id="476fd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="476fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="476fd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="476fd-126">Accept</span></span>|<span data-ttu-id="476fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="476fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="476fd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="476fd-128">Request body</span></span>
<span data-ttu-id="476fd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="476fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="476fd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="476fd-130">Response</span></span>
<span data-ttu-id="476fd-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="476fd-131">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="476fd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="476fd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="476fd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="476fd-133">Request</span></span>
<span data-ttu-id="476fd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="476fd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="476fd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="476fd-135">Response</span></span>
<span data-ttu-id="476fd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="476fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```






