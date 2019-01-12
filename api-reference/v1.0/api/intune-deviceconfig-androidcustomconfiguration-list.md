---
title: Перечисление объектов androidCustomConfiguration
description: Перечисление свойств и связей объектов androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bce9463260fb71145bc7b0b8fa329d57c9ee1545
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977201"
---
# <a name="list-androidcustomconfigurations"></a><span data-ttu-id="18e37-103">Перечисление объектов androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="18e37-103">List androidCustomConfigurations</span></span>

> <span data-ttu-id="18e37-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18e37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18e37-105">Перечисление свойств и связей объектов [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18e37-105">List properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18e37-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18e37-106">Prerequisites</span></span>
<span data-ttu-id="18e37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e37-109">Permission type</span></span>|<span data-ttu-id="18e37-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e37-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18e37-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18e37-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18e37-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18e37-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18e37-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e37-114">Not supported.</span></span>|
|<span data-ttu-id="18e37-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18e37-115">Application</span></span>|<span data-ttu-id="18e37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e37-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18e37-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e37-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18e37-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e37-118">Request headers</span></span>
|<span data-ttu-id="18e37-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18e37-119">Header</span></span>|<span data-ttu-id="18e37-120">Значение</span><span class="sxs-lookup"><span data-stu-id="18e37-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18e37-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e37-121">Authorization</span></span>|<span data-ttu-id="18e37-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18e37-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18e37-123">Accept</span><span class="sxs-lookup"><span data-stu-id="18e37-123">Accept</span></span>|<span data-ttu-id="18e37-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18e37-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18e37-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18e37-125">Request body</span></span>
<span data-ttu-id="18e37-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18e37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18e37-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e37-127">Response</span></span>
<span data-ttu-id="18e37-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18e37-128">If successful, this method returns a `200 OK` response code and a collection of [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18e37-129">Пример</span><span class="sxs-lookup"><span data-stu-id="18e37-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="18e37-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e37-130">Request</span></span>
<span data-ttu-id="18e37-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e37-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18e37-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="18e37-132">Response</span></span>
<span data-ttu-id="18e37-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18e37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCustomConfiguration",
      "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



