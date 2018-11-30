---
title: Список androidWorkProfileCustomConfigurations
description: Свойства списка и связей объектов androidWorkProfileCustomConfiguration.
ms.openlocfilehash: 419cc4fa47e99691beb65dfbbf83c97df445cc4b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026176"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="16fb3-103">Список androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="16fb3-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="16fb3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16fb3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16fb3-105">Свойства списка и связей объектов [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="16fb3-105">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16fb3-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16fb3-106">Prerequisites</span></span>
<span data-ttu-id="16fb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16fb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16fb3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16fb3-109">Permission type</span></span>|<span data-ttu-id="16fb3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16fb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16fb3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16fb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16fb3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16fb3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="16fb3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16fb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16fb3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16fb3-114">Not supported.</span></span>|
|<span data-ttu-id="16fb3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16fb3-115">Application</span></span>|<span data-ttu-id="16fb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16fb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16fb3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16fb3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16fb3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16fb3-118">Request headers</span></span>
|<span data-ttu-id="16fb3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16fb3-119">Header</span></span>|<span data-ttu-id="16fb3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="16fb3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16fb3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16fb3-121">Authorization</span></span>|<span data-ttu-id="16fb3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16fb3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16fb3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="16fb3-123">Accept</span></span>|<span data-ttu-id="16fb3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="16fb3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16fb3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16fb3-125">Request body</span></span>
<span data-ttu-id="16fb3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16fb3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16fb3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="16fb3-127">Response</span></span>
<span data-ttu-id="16fb3-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16fb3-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16fb3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="16fb3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="16fb3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="16fb3-130">Request</span></span>
<span data-ttu-id="16fb3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16fb3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="16fb3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="16fb3-132">Response</span></span>
<span data-ttu-id="16fb3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="16fb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

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
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```



