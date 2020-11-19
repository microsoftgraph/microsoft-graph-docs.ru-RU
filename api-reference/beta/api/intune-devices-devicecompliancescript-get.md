---
title: Получение Девицекомплианцескрипт
description: Чтение свойств и связей объекта Девицекомплианцескрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a3ea3289d1b19c6ce12770832fa9072f0834a0d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229179"
---
# <a name="get-devicecompliancescript"></a><span data-ttu-id="c4ff0-103">Получение Девицекомплианцескрипт</span><span class="sxs-lookup"><span data-stu-id="c4ff0-103">Get deviceComplianceScript</span></span>

<span data-ttu-id="c4ff0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ff0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4ff0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ff0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ff0-107">Чтение свойств и связей объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ff0-107">Read properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ff0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4ff0-108">Prerequisites</span></span>
<span data-ttu-id="c4ff0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ff0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ff0-111">Permission type</span></span>|<span data-ttu-id="c4ff0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4ff0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ff0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4ff0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ff0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4ff0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c4ff0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4ff0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ff0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-116">Not supported.</span></span>|
|<span data-ttu-id="c4ff0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4ff0-117">Application</span></span>|<span data-ttu-id="c4ff0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4ff0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ff0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4ff0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4ff0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4ff0-120">Optional query parameters</span></span>
<span data-ttu-id="c4ff0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4ff0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4ff0-122">Request headers</span></span>
|<span data-ttu-id="c4ff0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4ff0-123">Header</span></span>|<span data-ttu-id="c4ff0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c4ff0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ff0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4ff0-125">Authorization</span></span>|<span data-ttu-id="c4ff0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ff0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c4ff0-127">Accept</span></span>|<span data-ttu-id="c4ff0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ff0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ff0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4ff0-129">Request body</span></span>
<span data-ttu-id="c4ff0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ff0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ff0-131">Response</span></span>
<span data-ttu-id="c4ff0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-132">If successful, this method returns a `200 OK` response code and [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ff0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c4ff0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ff0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ff0-134">Request</span></span>
<span data-ttu-id="c4ff0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

### <a name="response"></a><span data-ttu-id="c4ff0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ff0-136">Response</span></span>
<span data-ttu-id="c4ff0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4ff0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 641

{
  "value": {
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
}
```




