---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0606ca724e19ee6578cb33ae0f786ae29432ed7c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277180"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="3cfb6-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="3cfb6-103">List windowsInformationProtectionAppLockerFiles</span></span>

<span data-ttu-id="3cfb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cfb6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cfb6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cfb6-107">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="3cfb6-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cfb6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3cfb6-108">Prerequisites</span></span>
<span data-ttu-id="3cfb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cfb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cfb6-111">Permission type</span></span>|<span data-ttu-id="3cfb6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cfb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cfb6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cfb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cfb6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cfb6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3cfb6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cfb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cfb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-116">Not supported.</span></span>|
|<span data-ttu-id="3cfb6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cfb6-117">Application</span></span>|<span data-ttu-id="3cfb6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cfb6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cfb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfb6-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3cfb6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3cfb6-120">Request headers</span></span>
|<span data-ttu-id="3cfb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cfb6-121">Header</span></span>|<span data-ttu-id="3cfb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3cfb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cfb6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cfb6-123">Authorization</span></span>|<span data-ttu-id="3cfb6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cfb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3cfb6-125">Accept</span></span>|<span data-ttu-id="3cfb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cfb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cfb6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cfb6-127">Request body</span></span>
<span data-ttu-id="3cfb6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cfb6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cfb6-129">Response</span></span>
<span data-ttu-id="3cfb6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cfb6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3cfb6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cfb6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cfb6-132">Request</span></span>
<span data-ttu-id="3cfb6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="3cfb6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cfb6-134">Response</span></span>
<span data-ttu-id="3cfb6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cfb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




