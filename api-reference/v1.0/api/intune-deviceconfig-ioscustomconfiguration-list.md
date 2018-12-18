---
title: Перечисление объектов iosCustomConfiguration
description: Список свойств и связей объектов iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 09a0d9a22c124bdc4c5d9532b712b6ece0ba5987
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352313"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="3c0cd-103">Перечисление объектов iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c0cd-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="3c0cd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c0cd-105">Список свойств и связей объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c0cd-105">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c0cd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c0cd-106">Prerequisites</span></span>
<span data-ttu-id="3c0cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c0cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c0cd-109">Permission type</span></span>|<span data-ttu-id="3c0cd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c0cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c0cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c0cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c0cd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c0cd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c0cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c0cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c0cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-114">Not supported.</span></span>|
|<span data-ttu-id="3c0cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c0cd-115">Application</span></span>|<span data-ttu-id="3c0cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c0cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c0cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c0cd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c0cd-118">Request headers</span></span>
|<span data-ttu-id="3c0cd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c0cd-119">Header</span></span>|<span data-ttu-id="3c0cd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3c0cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c0cd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c0cd-121">Authorization</span></span>|<span data-ttu-id="3c0cd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c0cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c0cd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3c0cd-123">Accept</span></span>|<span data-ttu-id="3c0cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c0cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0cd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c0cd-125">Request body</span></span>
<span data-ttu-id="3c0cd-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c0cd-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c0cd-127">Response</span></span>
<span data-ttu-id="3c0cd-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-128">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c0cd-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3c0cd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c0cd-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c0cd-130">Request</span></span>
<span data-ttu-id="3c0cd-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3c0cd-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c0cd-132">Response</span></span>
<span data-ttu-id="3c0cd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c0cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```



