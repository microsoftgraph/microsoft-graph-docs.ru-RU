---
title: Перечисление объектов iosCertificateProfile
description: Список свойств и связей объектов iosCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50ebd03e6c4ac298aae0ef3112a87eb307c1866b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753890"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="49b5a-103">Перечисление объектов iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="49b5a-103">List iosCertificateProfiles</span></span>

<span data-ttu-id="49b5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49b5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49b5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49b5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49b5a-106">Список свойств и связей объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="49b5a-106">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49b5a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49b5a-107">Prerequisites</span></span>
<span data-ttu-id="49b5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49b5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49b5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49b5a-110">Permission type</span></span>|<span data-ttu-id="49b5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49b5a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49b5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49b5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49b5a-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b5a-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49b5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49b5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49b5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b5a-115">Not supported.</span></span>|
|<span data-ttu-id="49b5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="49b5a-116">Application</span></span>|<span data-ttu-id="49b5a-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b5a-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49b5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49b5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49b5a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49b5a-119">Request headers</span></span>
|<span data-ttu-id="49b5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49b5a-120">Header</span></span>|<span data-ttu-id="49b5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="49b5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49b5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49b5a-122">Authorization</span></span>|<span data-ttu-id="49b5a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49b5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49b5a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="49b5a-124">Accept</span></span>|<span data-ttu-id="49b5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49b5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49b5a-126">Request body</span></span>
<span data-ttu-id="49b5a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49b5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49b5a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="49b5a-128">Response</span></span>
<span data-ttu-id="49b5a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49b5a-129">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b5a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="49b5a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49b5a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="49b5a-131">Request</span></span>
<span data-ttu-id="49b5a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49b5a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="49b5a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="49b5a-133">Response</span></span>
<span data-ttu-id="49b5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49b5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




