---
title: Перечисление объектов detectedApp
description: Список свойств и связей объектов detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9e09e7d63e550d86ceb797b8907fa2fa9e9db42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021048"
---
# <a name="list-detectedapps"></a><span data-ttu-id="c4eab-103">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="c4eab-103">List detectedApps</span></span>

> <span data-ttu-id="c4eab-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4eab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4eab-105">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4eab-105">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4eab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c4eab-106">Prerequisites</span></span>
<span data-ttu-id="c4eab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4eab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4eab-109">Permission type</span></span>|<span data-ttu-id="c4eab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4eab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4eab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4eab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4eab-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4eab-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c4eab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4eab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4eab-114">Not supported.</span></span>|
|<span data-ttu-id="c4eab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4eab-115">Application</span></span>|<span data-ttu-id="c4eab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4eab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4eab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4eab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="c4eab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4eab-118">Request headers</span></span>
|<span data-ttu-id="c4eab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4eab-119">Header</span></span>|<span data-ttu-id="c4eab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c4eab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4eab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4eab-121">Authorization</span></span>|<span data-ttu-id="c4eab-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4eab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4eab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c4eab-123">Accept</span></span>|<span data-ttu-id="c4eab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c4eab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4eab-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4eab-125">Request body</span></span>
<span data-ttu-id="c4eab-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4eab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4eab-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4eab-127">Response</span></span>
<span data-ttu-id="c4eab-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune-devices-detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4eab-128">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4eab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c4eab-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4eab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4eab-130">Request</span></span>
<span data-ttu-id="c4eab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4eab-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="c4eab-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eab-132">Response</span></span>
<span data-ttu-id="c4eab-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4eab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



