---
title: Список androidWorkProfileCustomConfigurations
description: Список свойств и связей объектов AndroidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fac08a8a30f0e743d7a5a2643ec1d86f8fba85e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757159"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="136f1-103">Список androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="136f1-103">List androidWorkProfileCustomConfigurations</span></span>

<span data-ttu-id="136f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="136f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="136f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="136f1-106">Список свойств и связей [объектов AndroidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="136f1-106">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="136f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="136f1-107">Prerequisites</span></span>
<span data-ttu-id="136f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="136f1-110">Permission type</span></span>|<span data-ttu-id="136f1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="136f1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="136f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="136f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="136f1-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136f1-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="136f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="136f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="136f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="136f1-115">Not supported.</span></span>|
|<span data-ttu-id="136f1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="136f1-116">Application</span></span>|<span data-ttu-id="136f1-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136f1-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="136f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="136f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="136f1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="136f1-119">Request headers</span></span>
|<span data-ttu-id="136f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="136f1-120">Header</span></span>|<span data-ttu-id="136f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="136f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="136f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="136f1-122">Authorization</span></span>|<span data-ttu-id="136f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="136f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="136f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="136f1-124">Accept</span></span>|<span data-ttu-id="136f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="136f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="136f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="136f1-126">Request body</span></span>
<span data-ttu-id="136f1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="136f1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136f1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="136f1-128">Response</span></span>
<span data-ttu-id="136f1-129">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="136f1-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="136f1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="136f1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="136f1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="136f1-131">Request</span></span>
<span data-ttu-id="136f1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="136f1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="136f1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="136f1-133">Response</span></span>
<span data-ttu-id="136f1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="136f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSetting",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value"
        }
      ]
    }
  ]
}
```




