---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8dd7588cef765035dfaaac07c55c90bd210feed4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465534"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="d93de-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="d93de-103">List windowsInformationProtectionAppLockerFiles</span></span>

<span data-ttu-id="d93de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d93de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d93de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93de-107">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="d93de-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93de-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d93de-108">Prerequisites</span></span>
<span data-ttu-id="d93de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d93de-111">Permission type</span></span>|<span data-ttu-id="d93de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d93de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d93de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d93de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d93de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d93de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93de-116">Not supported.</span></span>|
|<span data-ttu-id="d93de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d93de-117">Application</span></span>|<span data-ttu-id="d93de-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93de-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d93de-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d93de-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d93de-120">Request headers</span></span>
|<span data-ttu-id="d93de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d93de-121">Header</span></span>|<span data-ttu-id="d93de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d93de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d93de-123">Authorization</span></span>|<span data-ttu-id="d93de-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d93de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d93de-125">Accept</span></span>|<span data-ttu-id="d93de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d93de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d93de-127">Request body</span></span>
<span data-ttu-id="d93de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d93de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d93de-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d93de-129">Response</span></span>
<span data-ttu-id="d93de-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d93de-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d93de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d93de-132">Request</span></span>
<span data-ttu-id="d93de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d93de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="d93de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d93de-134">Response</span></span>
<span data-ttu-id="d93de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d93de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



