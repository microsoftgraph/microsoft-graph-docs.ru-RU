---
title: Список Виндовсфониасемаилпрофилеконфигуратионс
description: Список свойств и связей объектов Виндовсфониасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd017c17b7333376eb8c8f7bd28d8e6b919a9d00
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917522"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="fb992-103">Список Виндовсфониасемаилпрофилеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="fb992-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

> <span data-ttu-id="fb992-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb992-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb992-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb992-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb992-106">Список свойств и связей объектов [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fb992-106">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb992-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb992-107">Prerequisites</span></span>
<span data-ttu-id="fb992-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb992-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb992-110">Permission type</span></span>|<span data-ttu-id="fb992-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb992-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb992-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb992-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb992-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb992-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb992-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb992-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb992-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb992-115">Not supported.</span></span>|
|<span data-ttu-id="fb992-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb992-116">Application</span></span>|<span data-ttu-id="fb992-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb992-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb992-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb992-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb992-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb992-119">Request headers</span></span>
|<span data-ttu-id="fb992-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb992-120">Header</span></span>|<span data-ttu-id="fb992-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fb992-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb992-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb992-122">Authorization</span></span>|<span data-ttu-id="fb992-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb992-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb992-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fb992-124">Accept</span></span>|<span data-ttu-id="fb992-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb992-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb992-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb992-126">Request body</span></span>
<span data-ttu-id="fb992-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb992-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb992-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb992-128">Response</span></span>
<span data-ttu-id="fb992-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb992-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb992-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb992-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb992-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb992-131">Request</span></span>
<span data-ttu-id="fb992-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb992-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fb992-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb992-133">Response</span></span>
<span data-ttu-id="fb992-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb992-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1099

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
      "id": "554f402a-402a-554f-2a40-4f552a404f55",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value",
      "accountName": "Account Name value",
      "applyOnlyToWindowsPhone81": true,
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSsl": true
    }
  ]
}
```




