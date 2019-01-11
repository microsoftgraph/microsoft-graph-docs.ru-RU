---
title: Список deviceManagementScripts
description: Свойства списка и связей объектов deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c98ed25e43a0bb7990f900de816ee54a44c3da7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863639"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="34252-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="34252-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="34252-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34252-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34252-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34252-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34252-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="34252-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34252-107">Свойства списка и связей объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="34252-107">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34252-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34252-108">Prerequisites</span></span>
<span data-ttu-id="34252-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34252-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34252-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34252-111">Permission type</span></span>|<span data-ttu-id="34252-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34252-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34252-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34252-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34252-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34252-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="34252-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34252-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34252-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34252-116">Not supported.</span></span>|
|<span data-ttu-id="34252-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34252-117">Application</span></span>|<span data-ttu-id="34252-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34252-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34252-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34252-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="34252-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34252-120">Request headers</span></span>
|<span data-ttu-id="34252-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34252-121">Header</span></span>|<span data-ttu-id="34252-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34252-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34252-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34252-123">Authorization</span></span>|<span data-ttu-id="34252-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34252-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34252-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34252-125">Accept</span></span>|<span data-ttu-id="34252-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34252-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34252-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34252-127">Request body</span></span>
<span data-ttu-id="34252-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34252-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34252-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="34252-129">Response</span></span>
<span data-ttu-id="34252-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34252-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34252-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34252-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="34252-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34252-132">Request</span></span>
<span data-ttu-id="34252-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34252-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="34252-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="34252-134">Response</span></span>
<span data-ttu-id="34252-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34252-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

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
      "fileName": "File Name value"
    }
  ]
}
```





