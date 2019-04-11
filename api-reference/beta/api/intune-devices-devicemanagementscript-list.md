---
title: Список deviceManagementScripts
description: Список свойств и связей объектов deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ceff08ba72eb4dace69e2017b1b513bd456e20a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799995"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="6b951-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="6b951-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="6b951-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b951-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b951-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b951-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b951-106">Список свойств и связей объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6b951-106">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b951-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b951-107">Prerequisites</span></span>
<span data-ttu-id="6b951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b951-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b951-110">Permission type</span></span>|<span data-ttu-id="6b951-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b951-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b951-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b951-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b951-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b951-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6b951-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b951-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b951-115">Not supported.</span></span>|
|<span data-ttu-id="6b951-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b951-116">Application</span></span>|<span data-ttu-id="6b951-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b951-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b951-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b951-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="6b951-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b951-119">Request headers</span></span>
|<span data-ttu-id="6b951-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b951-120">Header</span></span>|<span data-ttu-id="6b951-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b951-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b951-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b951-122">Authorization</span></span>|<span data-ttu-id="6b951-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b951-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b951-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b951-124">Accept</span></span>|<span data-ttu-id="6b951-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b951-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b951-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b951-126">Request body</span></span>
<span data-ttu-id="6b951-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b951-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b951-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b951-128">Response</span></span>
<span data-ttu-id="6b951-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b951-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b951-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6b951-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b951-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b951-131">Request</span></span>
<span data-ttu-id="6b951-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b951-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="6b951-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b951-133">Response</span></span>
<span data-ttu-id="6b951-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b951-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "runAs32Bit": true
    }
  ]
}
```





