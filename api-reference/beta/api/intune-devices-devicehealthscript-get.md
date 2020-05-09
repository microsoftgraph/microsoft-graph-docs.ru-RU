---
title: Получение Девицехеалсскрипт
description: Чтение свойств и связей объекта Девицехеалсскрипт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b4e764893d8944971c0ceff8b9fbc647bf8958a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177039"
---
# <a name="get-devicehealthscript"></a><span data-ttu-id="ca3fe-103">Получение Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="ca3fe-103">Get deviceHealthScript</span></span>

<span data-ttu-id="ca3fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca3fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3fe-107">Чтение свойств и связей объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="ca3fe-107">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca3fe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca3fe-108">Prerequisites</span></span>
<span data-ttu-id="ca3fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca3fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca3fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3fe-111">Permission type</span></span>|<span data-ttu-id="ca3fe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca3fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca3fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca3fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca3fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca3fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca3fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca3fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca3fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-116">Not supported.</span></span>|
|<span data-ttu-id="ca3fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca3fe-117">Application</span></span>|<span data-ttu-id="ca3fe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca3fe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca3fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca3fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca3fe-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca3fe-120">Optional query parameters</span></span>
<span data-ttu-id="ca3fe-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca3fe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca3fe-122">Request headers</span></span>
|<span data-ttu-id="ca3fe-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca3fe-123">Header</span></span>|<span data-ttu-id="ca3fe-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ca3fe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca3fe-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca3fe-125">Authorization</span></span>|<span data-ttu-id="ca3fe-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca3fe-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ca3fe-127">Accept</span></span>|<span data-ttu-id="ca3fe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ca3fe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca3fe-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca3fe-129">Request body</span></span>
<span data-ttu-id="ca3fe-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca3fe-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca3fe-131">Response</span></span>
<span data-ttu-id="ca3fe-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-132">If successful, this method returns a `200 OK` response code and [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca3fe-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ca3fe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca3fe-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3fe-134">Request</span></span>
<span data-ttu-id="ca3fe-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

### <a name="response"></a><span data-ttu-id="ca3fe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3fe-136">Response</span></span>
<span data-ttu-id="ca3fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca3fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1488

{
  "value": {
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
    ],
    "isGlobalScript": true,
    "highestAvailableVersion": "Highest Available Version value",
    "detectionScriptParameters": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
        "name": "Name value",
        "description": "Description value",
        "isRequired": true,
        "applyDefaultValueWhenNotAssigned": true,
        "defaultValue": "Default Value value"
      }
    ],
    "remediationScriptParameters": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
        "name": "Name value",
        "description": "Description value",
        "isRequired": true,
        "applyDefaultValueWhenNotAssigned": true,
        "defaultValue": "Default Value value"
      }
    ]
  }
}
```



