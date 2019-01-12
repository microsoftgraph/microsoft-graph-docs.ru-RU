---
title: Перечисление объектов deviceConfiguration
description: Список свойств и связей объектов deviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ebeb789bc9124176e63db6cb8b653ea232c49a24
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917547"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="302d8-103">Перечисление объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="302d8-103">List deviceConfigurations</span></span>

> <span data-ttu-id="302d8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="302d8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="302d8-105">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="302d8-105">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="302d8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="302d8-106">Prerequisites</span></span>
<span data-ttu-id="302d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="302d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="302d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="302d8-109">Permission type</span></span>|<span data-ttu-id="302d8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="302d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="302d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="302d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="302d8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="302d8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="302d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="302d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="302d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="302d8-114">Not supported.</span></span>|
|<span data-ttu-id="302d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="302d8-115">Application</span></span>|<span data-ttu-id="302d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="302d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="302d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="302d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="302d8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="302d8-118">Request headers</span></span>
|<span data-ttu-id="302d8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="302d8-119">Header</span></span>|<span data-ttu-id="302d8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="302d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="302d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="302d8-121">Authorization</span></span>|<span data-ttu-id="302d8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="302d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="302d8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="302d8-123">Accept</span></span>|<span data-ttu-id="302d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="302d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="302d8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="302d8-125">Request body</span></span>
<span data-ttu-id="302d8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="302d8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="302d8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="302d8-127">Response</span></span>
<span data-ttu-id="302d8-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="302d8-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="302d8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="302d8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="302d8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="302d8-130">Request</span></span>
<span data-ttu-id="302d8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="302d8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="302d8-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="302d8-132">Response</span></span>
<span data-ttu-id="302d8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="302d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



