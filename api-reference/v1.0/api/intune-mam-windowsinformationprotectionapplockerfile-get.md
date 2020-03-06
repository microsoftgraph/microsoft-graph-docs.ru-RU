---
title: Получение объекта windowsInformationProtectionAppLockerFile
description: Чтение свойств и связей объекта windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8221533ce630be8a3615c4f46d2458fc2d5aa561
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512869"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c6574-103">Получение объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c6574-103">Get windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="c6574-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6574-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6574-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6574-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6574-106">Чтение свойств и связей объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c6574-106">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6574-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c6574-107">Prerequisites</span></span>
<span data-ttu-id="c6574-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6574-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6574-110">Permission type</span></span>|<span data-ttu-id="c6574-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6574-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6574-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6574-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6574-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6574-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c6574-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6574-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6574-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6574-115">Not supported.</span></span>|
|<span data-ttu-id="c6574-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6574-116">Application</span></span>|<span data-ttu-id="c6574-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6574-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6574-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6574-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6574-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6574-119">Optional query parameters</span></span>
<span data-ttu-id="c6574-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c6574-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6574-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6574-121">Request headers</span></span>
|<span data-ttu-id="c6574-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6574-122">Header</span></span>|<span data-ttu-id="c6574-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c6574-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6574-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6574-124">Authorization</span></span>|<span data-ttu-id="c6574-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6574-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6574-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c6574-126">Accept</span></span>|<span data-ttu-id="c6574-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c6574-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6574-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6574-128">Request body</span></span>
<span data-ttu-id="c6574-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6574-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6574-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6574-130">Response</span></span>
<span data-ttu-id="c6574-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6574-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6574-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c6574-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6574-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6574-133">Request</span></span>
<span data-ttu-id="c6574-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6574-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="c6574-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6574-135">Response</span></span>
<span data-ttu-id="c6574-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6574-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```




