---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f5a78b7c68cf038cff4a3681810b49cde0c36de
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942158"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="b04d9-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="b04d9-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="b04d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b04d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b04d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b04d9-106">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="b04d9-106">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b04d9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b04d9-107">Prerequisites</span></span>
<span data-ttu-id="b04d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b04d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b04d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b04d9-110">Permission type</span></span>|<span data-ttu-id="b04d9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b04d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b04d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b04d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b04d9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04d9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b04d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b04d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b04d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04d9-115">Not supported.</span></span>|
|<span data-ttu-id="b04d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b04d9-116">Application</span></span>|<span data-ttu-id="b04d9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04d9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b04d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b04d9-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b04d9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b04d9-119">Request headers</span></span>
|<span data-ttu-id="b04d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b04d9-120">Header</span></span>|<span data-ttu-id="b04d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b04d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b04d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b04d9-122">Authorization</span></span>|<span data-ttu-id="b04d9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b04d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b04d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b04d9-124">Accept</span></span>|<span data-ttu-id="b04d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b04d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b04d9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b04d9-126">Request body</span></span>
<span data-ttu-id="b04d9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b04d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b04d9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b04d9-128">Response</span></span>
<span data-ttu-id="b04d9-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b04d9-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b04d9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b04d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b04d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b04d9-131">Request</span></span>
<span data-ttu-id="b04d9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b04d9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="b04d9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b04d9-133">Response</span></span>
<span data-ttu-id="b04d9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b04d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





