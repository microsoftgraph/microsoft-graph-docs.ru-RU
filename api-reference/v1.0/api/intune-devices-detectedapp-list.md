---
title: Перечисление объектов detectedApp
description: Список свойств и связей объектов detectedApp.
ms.openlocfilehash: 1f56f00d9a872e0d6187522ec795d11ce292225a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026678"
---
# <a name="list-detectedapps"></a><span data-ttu-id="566ef-103">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="566ef-103">List detectedApps</span></span>

> <span data-ttu-id="566ef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="566ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="566ef-105">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="566ef-105">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="566ef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="566ef-106">Prerequisites</span></span>
<span data-ttu-id="566ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="566ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="566ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="566ef-109">Permission type</span></span>|<span data-ttu-id="566ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="566ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="566ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="566ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="566ef-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="566ef-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="566ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="566ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="566ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="566ef-114">Not supported.</span></span>|
|<span data-ttu-id="566ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="566ef-115">Application</span></span>|<span data-ttu-id="566ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="566ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="566ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="566ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="566ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="566ef-118">Request headers</span></span>
|<span data-ttu-id="566ef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="566ef-119">Header</span></span>|<span data-ttu-id="566ef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="566ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="566ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="566ef-121">Authorization</span></span>|<span data-ttu-id="566ef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="566ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="566ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="566ef-123">Accept</span></span>|<span data-ttu-id="566ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="566ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="566ef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="566ef-125">Request body</span></span>
<span data-ttu-id="566ef-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="566ef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="566ef-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="566ef-127">Response</span></span>
<span data-ttu-id="566ef-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune-devices-detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="566ef-128">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="566ef-129">Пример</span><span class="sxs-lookup"><span data-stu-id="566ef-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="566ef-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="566ef-130">Request</span></span>
<span data-ttu-id="566ef-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="566ef-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="566ef-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="566ef-132">Response</span></span>
<span data-ttu-id="566ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="566ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```



