---
title: Получение Андроидворкпрофилиасемаилпрофилебасе
description: Чтение свойств и связей объекта Андроидворкпрофилиасемаилпрофилебасе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e28fbc7bcd56d1ebced5d979c0b83a542ac0535
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690009"
---
# <a name="get-androidworkprofileeasemailprofilebase"></a><span data-ttu-id="38045-103">Получение Андроидворкпрофилиасемаилпрофилебасе</span><span class="sxs-lookup"><span data-stu-id="38045-103">Get androidWorkProfileEasEmailProfileBase</span></span>

<span data-ttu-id="38045-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38045-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38045-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38045-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38045-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38045-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38045-107">Чтение свойств и связей объекта [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="38045-107">Read properties and relationships of the [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38045-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38045-108">Prerequisites</span></span>
<span data-ttu-id="38045-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38045-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38045-111">Permission type</span></span>|<span data-ttu-id="38045-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38045-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38045-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38045-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38045-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38045-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38045-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38045-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38045-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38045-116">Not supported.</span></span>|
|<span data-ttu-id="38045-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38045-117">Application</span></span>|<span data-ttu-id="38045-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38045-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38045-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38045-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38045-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38045-120">Optional query parameters</span></span>
<span data-ttu-id="38045-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38045-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38045-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38045-122">Request headers</span></span>
|<span data-ttu-id="38045-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38045-123">Header</span></span>|<span data-ttu-id="38045-124">Значение</span><span class="sxs-lookup"><span data-stu-id="38045-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38045-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38045-125">Authorization</span></span>|<span data-ttu-id="38045-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38045-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38045-127">Accept</span><span class="sxs-lookup"><span data-stu-id="38045-127">Accept</span></span>|<span data-ttu-id="38045-128">application/json</span><span class="sxs-lookup"><span data-stu-id="38045-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38045-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38045-129">Request body</span></span>
<span data-ttu-id="38045-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38045-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38045-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="38045-131">Response</span></span>
<span data-ttu-id="38045-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38045-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38045-133">Пример</span><span class="sxs-lookup"><span data-stu-id="38045-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="38045-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="38045-134">Request</span></span>
<span data-ttu-id="38045-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38045-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="38045-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="38045-136">Response</span></span>
<span data-ttu-id="38045-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38045-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1533

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileEasEmailProfileBase",
    "id": "5d74f295-f295-5d74-95f2-745d95f2745d",
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
    "version": 7,
    "authenticationMethod": "certificate",
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "hostName": "Host Name value",
    "requireSsl": true,
    "usernameSource": "userPrincipalName"
  }
}
```





