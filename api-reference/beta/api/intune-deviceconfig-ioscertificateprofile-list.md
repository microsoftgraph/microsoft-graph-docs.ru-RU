---
title: Перечисление объектов iosCertificateProfile
description: Список свойств и связей объектов iosCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c328e0a13792fbb2e5b6c29f06481a09abf4edc5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206331"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="30aca-103">Перечисление объектов iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="30aca-103">List iosCertificateProfiles</span></span>

<span data-ttu-id="30aca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30aca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30aca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30aca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30aca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30aca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30aca-107">Список свойств и связей объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="30aca-107">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30aca-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30aca-108">Prerequisites</span></span>
<span data-ttu-id="30aca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30aca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30aca-111">Permission type</span></span>|<span data-ttu-id="30aca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30aca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30aca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30aca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30aca-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30aca-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30aca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30aca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30aca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30aca-116">Not supported.</span></span>|
|<span data-ttu-id="30aca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="30aca-117">Application</span></span>|<span data-ttu-id="30aca-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30aca-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30aca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30aca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="30aca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30aca-120">Request headers</span></span>
|<span data-ttu-id="30aca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30aca-121">Header</span></span>|<span data-ttu-id="30aca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30aca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30aca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30aca-123">Authorization</span></span>|<span data-ttu-id="30aca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30aca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30aca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30aca-125">Accept</span></span>|<span data-ttu-id="30aca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30aca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30aca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30aca-127">Request body</span></span>
<span data-ttu-id="30aca-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30aca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30aca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="30aca-129">Response</span></span>
<span data-ttu-id="30aca-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30aca-130">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30aca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="30aca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30aca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="30aca-132">Request</span></span>
<span data-ttu-id="30aca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30aca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="30aca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30aca-134">Response</span></span>
<span data-ttu-id="30aca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1357

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




