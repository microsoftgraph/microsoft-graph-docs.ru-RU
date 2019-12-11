---
title: Список Девицехеалсскриптс
description: Список свойств и связей объектов Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4315f4b5d0a3836620c25e0c8688a029680e71e3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945139"
---
# <a name="list-devicehealthscripts"></a><span data-ttu-id="00119-103">Список Девицехеалсскриптс</span><span class="sxs-lookup"><span data-stu-id="00119-103">List deviceHealthScripts</span></span>

> <span data-ttu-id="00119-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00119-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00119-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00119-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00119-106">Список свойств и связей объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="00119-106">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00119-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00119-107">Prerequisites</span></span>
<span data-ttu-id="00119-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00119-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00119-110">Permission type</span></span>|<span data-ttu-id="00119-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00119-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00119-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00119-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00119-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="00119-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="00119-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00119-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00119-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00119-115">Not supported.</span></span>|
|<span data-ttu-id="00119-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00119-116">Application</span></span>|<span data-ttu-id="00119-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="00119-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00119-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00119-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="00119-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00119-119">Request headers</span></span>
|<span data-ttu-id="00119-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00119-120">Header</span></span>|<span data-ttu-id="00119-121">Значение</span><span class="sxs-lookup"><span data-stu-id="00119-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00119-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00119-122">Authorization</span></span>|<span data-ttu-id="00119-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00119-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00119-124">Accept</span><span class="sxs-lookup"><span data-stu-id="00119-124">Accept</span></span>|<span data-ttu-id="00119-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00119-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00119-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00119-126">Request body</span></span>
<span data-ttu-id="00119-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00119-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00119-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="00119-128">Response</span></span>
<span data-ttu-id="00119-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00119-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00119-130">Пример</span><span class="sxs-lookup"><span data-stu-id="00119-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00119-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="00119-131">Request</span></span>
<span data-ttu-id="00119-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00119-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a><span data-ttu-id="00119-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="00119-133">Response</span></span>
<span data-ttu-id="00119-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00119-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 752

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





