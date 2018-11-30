---
title: Список windowsPhoneEASEmailProfileConfigurations
description: Свойства списка и связей объектов windowsPhoneEASEmailProfileConfiguration.
ms.openlocfilehash: 89b43ef2dcbef5687567022ba7beb990709d63fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078404"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="f25d3-103">Список windowsPhoneEASEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="f25d3-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

> <span data-ttu-id="f25d3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f25d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f25d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f25d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f25d3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f25d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f25d3-107">Свойства списка и связей объектов [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f25d3-107">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f25d3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f25d3-108">Prerequisites</span></span>
<span data-ttu-id="f25d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f25d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f25d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f25d3-111">Permission type</span></span>|<span data-ttu-id="f25d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f25d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f25d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f25d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f25d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f25d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f25d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f25d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f25d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f25d3-116">Not supported.</span></span>|
|<span data-ttu-id="f25d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f25d3-117">Application</span></span>|<span data-ttu-id="f25d3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f25d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f25d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f25d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f25d3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f25d3-120">Request headers</span></span>
|<span data-ttu-id="f25d3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f25d3-121">Header</span></span>|<span data-ttu-id="f25d3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f25d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f25d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f25d3-123">Authorization</span></span>|<span data-ttu-id="f25d3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f25d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f25d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f25d3-125">Accept</span></span>|<span data-ttu-id="f25d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f25d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f25d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f25d3-127">Request body</span></span>
<span data-ttu-id="f25d3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f25d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f25d3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f25d3-129">Response</span></span>
<span data-ttu-id="f25d3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f25d3-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f25d3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f25d3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f25d3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f25d3-132">Request</span></span>
<span data-ttu-id="f25d3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f25d3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f25d3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f25d3-134">Response</span></span>
<span data-ttu-id="f25d3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f25d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





