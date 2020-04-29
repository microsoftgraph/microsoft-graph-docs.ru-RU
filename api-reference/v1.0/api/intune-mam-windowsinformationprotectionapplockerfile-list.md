---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 890d3eaef84879404c4dbcb44831ba1f2c241561
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450142"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="86a6f-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="86a6f-103">List windowsInformationProtectionAppLockerFiles</span></span>

<span data-ttu-id="86a6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86a6f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86a6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a6f-106">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="86a6f-106">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a6f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="86a6f-107">Prerequisites</span></span>
<span data-ttu-id="86a6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86a6f-110">Permission type</span></span>|<span data-ttu-id="86a6f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86a6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86a6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a6f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a6f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86a6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86a6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a6f-115">Not supported.</span></span>|
|<span data-ttu-id="86a6f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86a6f-116">Application</span></span>|<span data-ttu-id="86a6f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86a6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="86a6f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86a6f-119">Request headers</span></span>
|<span data-ttu-id="86a6f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86a6f-120">Header</span></span>|<span data-ttu-id="86a6f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86a6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a6f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86a6f-122">Authorization</span></span>|<span data-ttu-id="86a6f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86a6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a6f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86a6f-124">Accept</span></span>|<span data-ttu-id="86a6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86a6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a6f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86a6f-126">Request body</span></span>
<span data-ttu-id="86a6f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86a6f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86a6f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="86a6f-128">Response</span></span>
<span data-ttu-id="86a6f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86a6f-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a6f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="86a6f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a6f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="86a6f-131">Request</span></span>
<span data-ttu-id="86a6f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86a6f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="86a6f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a6f-133">Response</span></span>
<span data-ttu-id="86a6f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86a6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```






