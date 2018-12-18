---
title: Список importedDeviceIdentityResults
description: Свойства списка и связей объектов importedDeviceIdentityResult.
author: tfitzmac
ms.openlocfilehash: e7d876c649d3f088d238e2fc804e61fbcddbf8b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355603"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="a5197-103">Список importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="a5197-103">List importedDeviceIdentityResults</span></span>

> <span data-ttu-id="a5197-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5197-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5197-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5197-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a5197-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5197-107">Свойства списка и связей объектов [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="a5197-107">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5197-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a5197-108">Prerequisites</span></span>
<span data-ttu-id="a5197-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5197-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5197-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5197-111">Permission type</span></span>|<span data-ttu-id="a5197-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5197-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5197-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5197-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5197-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5197-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a5197-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5197-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5197-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5197-116">Not supported.</span></span>|
|<span data-ttu-id="a5197-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5197-117">Application</span></span>|<span data-ttu-id="a5197-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5197-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5197-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5197-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a5197-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5197-120">Request headers</span></span>
|<span data-ttu-id="a5197-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5197-121">Header</span></span>|<span data-ttu-id="a5197-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5197-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5197-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5197-123">Authorization</span></span>|<span data-ttu-id="a5197-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a5197-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5197-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5197-125">Accept</span></span>|<span data-ttu-id="a5197-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5197-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5197-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5197-127">Request body</span></span>
<span data-ttu-id="a5197-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5197-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5197-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5197-129">Response</span></span>
<span data-ttu-id="a5197-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a5197-130">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5197-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a5197-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5197-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5197-132">Request</span></span>
<span data-ttu-id="a5197-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5197-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="a5197-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5197-134">Response</span></span>
<span data-ttu-id="a5197-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a5197-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





