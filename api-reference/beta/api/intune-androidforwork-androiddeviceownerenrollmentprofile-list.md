---
title: Список Андроиддевицеовнеренроллментпрофилес
description: Список свойств и связей объектов Андроиддевицеовнеренроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d53cf005f458d44da27027785f7c00efbb55ac12
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255177"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="57486-103">Список Андроиддевицеовнеренроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="57486-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

<span data-ttu-id="57486-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57486-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57486-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57486-107">Список свойств и связей объектов [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="57486-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57486-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57486-108">Prerequisites</span></span>
<span data-ttu-id="57486-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57486-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57486-111">Permission type</span></span>|<span data-ttu-id="57486-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57486-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57486-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57486-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57486-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57486-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57486-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57486-116">Not supported.</span></span>|
|<span data-ttu-id="57486-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="57486-117">Application</span></span>|<span data-ttu-id="57486-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57486-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57486-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="57486-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57486-120">Request headers</span></span>
|<span data-ttu-id="57486-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57486-121">Header</span></span>|<span data-ttu-id="57486-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57486-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57486-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57486-123">Authorization</span></span>|<span data-ttu-id="57486-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57486-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57486-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57486-125">Accept</span></span>|<span data-ttu-id="57486-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57486-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57486-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57486-127">Request body</span></span>
<span data-ttu-id="57486-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57486-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57486-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="57486-129">Response</span></span>
<span data-ttu-id="57486-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57486-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57486-131">Пример</span><span class="sxs-lookup"><span data-stu-id="57486-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="57486-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="57486-132">Request</span></span>
<span data-ttu-id="57486-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57486-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="57486-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="57486-134">Response</span></span>
<span data-ttu-id="57486-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57486-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "enrollmentMode": "corporateOwnedFullyManaged",
      "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
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
      },
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




