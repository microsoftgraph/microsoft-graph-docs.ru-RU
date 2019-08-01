---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e870c49c6c814d999c0159783fd7f454903b5bcb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020530"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="85e62-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="85e62-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="85e62-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85e62-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e62-105">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="85e62-105">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e62-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85e62-106">Prerequisites</span></span>
<span data-ttu-id="85e62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e62-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85e62-109">Permission type</span></span>|<span data-ttu-id="85e62-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85e62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e62-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85e62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85e62-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85e62-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="85e62-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85e62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e62-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e62-114">Not supported.</span></span>|
|<span data-ttu-id="85e62-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85e62-115">Application</span></span>|<span data-ttu-id="85e62-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e62-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85e62-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="85e62-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85e62-118">Request headers</span></span>
|<span data-ttu-id="85e62-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85e62-119">Header</span></span>|<span data-ttu-id="85e62-120">Значение</span><span class="sxs-lookup"><span data-stu-id="85e62-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e62-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85e62-121">Authorization</span></span>|<span data-ttu-id="85e62-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85e62-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e62-123">Accept</span><span class="sxs-lookup"><span data-stu-id="85e62-123">Accept</span></span>|<span data-ttu-id="85e62-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85e62-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e62-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85e62-125">Request body</span></span>
<span data-ttu-id="85e62-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85e62-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85e62-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="85e62-127">Response</span></span>
<span data-ttu-id="85e62-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85e62-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e62-129">Пример</span><span class="sxs-lookup"><span data-stu-id="85e62-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e62-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="85e62-130">Request</span></span>
<span data-ttu-id="85e62-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85e62-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="85e62-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="85e62-132">Response</span></span>
<span data-ttu-id="85e62-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85e62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



