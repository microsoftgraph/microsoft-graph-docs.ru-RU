---
title: Список Андроиддевицеовнеренроллментпрофилес
description: Список свойств и связей объектов Андроиддевицеовнеренроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16244072fd53cdf611c41fc03f5ed96ee0d6c7ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789355"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="24e21-103">Список Андроиддевицеовнеренроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="24e21-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="24e21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24e21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24e21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24e21-106">Список свойств и связей объектов [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="24e21-106">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24e21-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24e21-107">Prerequisites</span></span>
<span data-ttu-id="24e21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24e21-110">Permission type</span></span>|<span data-ttu-id="24e21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24e21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24e21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24e21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24e21-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24e21-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24e21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24e21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24e21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e21-115">Not supported.</span></span>|
|<span data-ttu-id="24e21-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24e21-116">Application</span></span>|<span data-ttu-id="24e21-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24e21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24e21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="24e21-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24e21-119">Request headers</span></span>
|<span data-ttu-id="24e21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24e21-120">Header</span></span>|<span data-ttu-id="24e21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="24e21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24e21-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24e21-122">Authorization</span></span>|<span data-ttu-id="24e21-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24e21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="24e21-124">Accept</span></span>|<span data-ttu-id="24e21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24e21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24e21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24e21-126">Request body</span></span>
<span data-ttu-id="24e21-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24e21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e21-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="24e21-128">Response</span></span>
<span data-ttu-id="24e21-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24e21-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24e21-130">Пример</span><span class="sxs-lookup"><span data-stu-id="24e21-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="24e21-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="24e21-131">Request</span></span>
<span data-ttu-id="24e21-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24e21-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="24e21-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e21-133">Response</span></span>
<span data-ttu-id="24e21-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24e21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "enrolledDeviceCount": 3,
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ]
}
```





