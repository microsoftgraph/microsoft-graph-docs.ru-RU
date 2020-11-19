---
title: Список Девицекомплианцескриптс
description: Список свойств и связей объектов Девицекомплианцескрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65d4d4500843b33959f7579ac996e3487e741822
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229028"
---
# <a name="list-devicecompliancescripts"></a><span data-ttu-id="a0599-103">Список Девицекомплианцескриптс</span><span class="sxs-lookup"><span data-stu-id="a0599-103">List deviceComplianceScripts</span></span>

<span data-ttu-id="a0599-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0599-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0599-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0599-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0599-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0599-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0599-107">Список свойств и связей объектов [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="a0599-107">List properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0599-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0599-108">Prerequisites</span></span>
<span data-ttu-id="a0599-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0599-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0599-111">Permission type</span></span>|<span data-ttu-id="a0599-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0599-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0599-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0599-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0599-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0599-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a0599-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0599-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0599-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0599-116">Not supported.</span></span>|
|<span data-ttu-id="a0599-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0599-117">Application</span></span>|<span data-ttu-id="a0599-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0599-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0599-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0599-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="a0599-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0599-120">Request headers</span></span>
|<span data-ttu-id="a0599-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0599-121">Header</span></span>|<span data-ttu-id="a0599-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a0599-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0599-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0599-123">Authorization</span></span>|<span data-ttu-id="a0599-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0599-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0599-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0599-125">Accept</span></span>|<span data-ttu-id="a0599-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0599-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0599-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0599-127">Request body</span></span>
<span data-ttu-id="a0599-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0599-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0599-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0599-129">Response</span></span>
<span data-ttu-id="a0599-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0599-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0599-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a0599-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0599-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0599-132">Request</span></span>
<span data-ttu-id="a0599-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0599-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
```

### <a name="response"></a><span data-ttu-id="a0599-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0599-134">Response</span></span>
<span data-ttu-id="a0599-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0599-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 685

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScript",
      "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
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




