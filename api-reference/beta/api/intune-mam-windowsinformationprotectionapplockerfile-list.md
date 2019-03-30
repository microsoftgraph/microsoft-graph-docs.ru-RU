---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e85388b8ed9e219bc5f2dbd8231e14f3a23254b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985489"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="c1a12-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c1a12-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="c1a12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1a12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1a12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a12-106">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c1a12-106">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1a12-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1a12-107">Prerequisites</span></span>
<span data-ttu-id="c1a12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a12-110">Permission type</span></span>|<span data-ttu-id="c1a12-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1a12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1a12-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1a12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1a12-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1a12-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1a12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1a12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a12-115">Not supported.</span></span>|
|<span data-ttu-id="c1a12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1a12-116">Application</span></span>|<span data-ttu-id="c1a12-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1a12-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c1a12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1a12-119">Request headers</span></span>
|<span data-ttu-id="c1a12-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1a12-120">Header</span></span>|<span data-ttu-id="c1a12-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1a12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1a12-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1a12-122">Authorization</span></span>|<span data-ttu-id="c1a12-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1a12-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1a12-124">Accept</span></span>|<span data-ttu-id="c1a12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a12-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1a12-126">Request body</span></span>
<span data-ttu-id="c1a12-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1a12-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1a12-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a12-128">Response</span></span>
<span data-ttu-id="c1a12-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1a12-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a12-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c1a12-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1a12-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a12-131">Request</span></span>
<span data-ttu-id="c1a12-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a12-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="c1a12-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a12-133">Response</span></span>
<span data-ttu-id="c1a12-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1a12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




