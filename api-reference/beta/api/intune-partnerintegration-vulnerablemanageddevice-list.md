---
title: Список Вулнераблеманажеддевицес
description: Список свойств и связей объектов Вулнераблеманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4775f421d9b12b8eafd27435880fb7bb3d855f93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257991"
---
# <a name="list-vulnerablemanageddevices"></a><span data-ttu-id="b1c77-103">Список Вулнераблеманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="b1c77-103">List vulnerableManagedDevices</span></span>

<span data-ttu-id="b1c77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1c77-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1c77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c77-107">Список свойств и связей объектов [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c77-107">List properties and relationships of the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1c77-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1c77-108">Prerequisites</span></span>
<span data-ttu-id="b1c77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c77-111">Permission type</span></span>|<span data-ttu-id="b1c77-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1c77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1c77-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1c77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1c77-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1c77-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b1c77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1c77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1c77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c77-116">Not supported.</span></span>|
|<span data-ttu-id="b1c77-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1c77-117">Application</span></span>|<span data-ttu-id="b1c77-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1c77-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1c77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1c77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="b1c77-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1c77-120">Request headers</span></span>
|<span data-ttu-id="b1c77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1c77-121">Header</span></span>|<span data-ttu-id="b1c77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1c77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1c77-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1c77-123">Authorization</span></span>|<span data-ttu-id="b1c77-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1c77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1c77-125">Accept</span></span>|<span data-ttu-id="b1c77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1c77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1c77-127">Request body</span></span>
<span data-ttu-id="b1c77-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1c77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1c77-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c77-129">Response</span></span>
<span data-ttu-id="b1c77-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c77-130">If successful, this method returns a `200 OK` response code and a collection of [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1c77-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b1c77-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1c77-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1c77-132">Request</span></span>
<span data-ttu-id="b1c77-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c77-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

### <a name="response"></a><span data-ttu-id="b1c77-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c77-134">Response</span></span>
<span data-ttu-id="b1c77-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1c77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
      "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
      "managedDeviceId": "Managed Device Id value",
      "displayName": "Display Name value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```




