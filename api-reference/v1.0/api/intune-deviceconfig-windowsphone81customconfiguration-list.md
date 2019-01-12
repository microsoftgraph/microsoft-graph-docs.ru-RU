---
title: Перечисление объектов windowsPhone81CustomConfiguration
description: Перечисление свойств и связей объектов windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b9d2e7641a0f2ae902b0ac310e36c0ce5678c054
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963950"
---
# <a name="list-windowsphone81customconfigurations"></a><span data-ttu-id="34914-103">Перечисление объектов windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="34914-103">List windowsPhone81CustomConfigurations</span></span>

> <span data-ttu-id="34914-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="34914-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34914-105">Перечисление свойств и связей объектов [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34914-105">List properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34914-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34914-106">Prerequisites</span></span>
<span data-ttu-id="34914-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34914-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34914-109">Permission type</span></span>|<span data-ttu-id="34914-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34914-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34914-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34914-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34914-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34914-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34914-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34914-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34914-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34914-114">Not supported.</span></span>|
|<span data-ttu-id="34914-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34914-115">Application</span></span>|<span data-ttu-id="34914-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34914-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34914-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34914-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34914-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34914-118">Request headers</span></span>
|<span data-ttu-id="34914-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34914-119">Header</span></span>|<span data-ttu-id="34914-120">Значение</span><span class="sxs-lookup"><span data-stu-id="34914-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34914-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34914-121">Authorization</span></span>|<span data-ttu-id="34914-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34914-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34914-123">Accept</span><span class="sxs-lookup"><span data-stu-id="34914-123">Accept</span></span>|<span data-ttu-id="34914-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34914-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34914-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34914-125">Request body</span></span>
<span data-ttu-id="34914-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34914-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34914-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="34914-127">Response</span></span>
<span data-ttu-id="34914-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34914-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34914-129">Пример</span><span class="sxs-lookup"><span data-stu-id="34914-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="34914-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="34914-130">Request</span></span>
<span data-ttu-id="34914-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34914-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="34914-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="34914-132">Response</span></span>
<span data-ttu-id="34914-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34914-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 678

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
      "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



