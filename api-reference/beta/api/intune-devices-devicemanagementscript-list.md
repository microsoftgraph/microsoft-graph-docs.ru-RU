---
title: Список deviceManagementScripts
description: Список свойств и связей объектов deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be5e92ef3d3a916d969443a2648da84f0641714c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967449"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="c6d99-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="c6d99-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="c6d99-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6d99-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6d99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6d99-106">Список свойств и связей объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d99-106">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6d99-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6d99-107">Prerequisites</span></span>
<span data-ttu-id="c6d99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6d99-110">Permission type</span></span>|<span data-ttu-id="c6d99-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6d99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6d99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6d99-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6d99-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c6d99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6d99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6d99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d99-115">Not supported.</span></span>|
|<span data-ttu-id="c6d99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6d99-116">Application</span></span>|<span data-ttu-id="c6d99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6d99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6d99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="c6d99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6d99-119">Request headers</span></span>
|<span data-ttu-id="c6d99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6d99-120">Header</span></span>|<span data-ttu-id="c6d99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c6d99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6d99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6d99-122">Authorization</span></span>|<span data-ttu-id="c6d99-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6d99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6d99-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c6d99-124">Accept</span></span>|<span data-ttu-id="c6d99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6d99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d99-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6d99-126">Request body</span></span>
<span data-ttu-id="c6d99-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6d99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6d99-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6d99-128">Response</span></span>
<span data-ttu-id="c6d99-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6d99-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6d99-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c6d99-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6d99-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6d99-131">Request</span></span>
<span data-ttu-id="c6d99-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6d99-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="c6d99-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6d99-133">Response</span></span>
<span data-ttu-id="c6d99-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6d99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




