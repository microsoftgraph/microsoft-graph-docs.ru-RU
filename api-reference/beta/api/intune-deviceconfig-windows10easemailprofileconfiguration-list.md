---
title: Список windows10EasEmailProfileConfigurations
description: Свойства списка и связей объектов windows10EasEmailProfileConfiguration.
ms.openlocfilehash: 9a5f10e0b57d2fa426434698392fe7741d68fb6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078042"
---
# <a name="list-windows10easemailprofileconfigurations"></a><span data-ttu-id="cbbf5-103">Список windows10EasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="cbbf5-103">List windows10EasEmailProfileConfigurations</span></span>

> <span data-ttu-id="cbbf5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbbf5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbbf5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbbf5-107">Свойства списка и связей объектов [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cbbf5-107">List properties and relationships of the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbbf5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cbbf5-108">Prerequisites</span></span>
<span data-ttu-id="cbbf5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbbf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbbf5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbbf5-111">Permission type</span></span>|<span data-ttu-id="cbbf5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbbf5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbbf5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbbf5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbbf5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbbf5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cbbf5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbbf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbbf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-116">Not supported.</span></span>|
|<span data-ttu-id="cbbf5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbbf5-117">Application</span></span>|<span data-ttu-id="cbbf5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbbf5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbbf5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cbbf5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbbf5-120">Request headers</span></span>
|<span data-ttu-id="cbbf5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbbf5-121">Header</span></span>|<span data-ttu-id="cbbf5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cbbf5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbbf5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbbf5-123">Authorization</span></span>|<span data-ttu-id="cbbf5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cbbf5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbbf5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cbbf5-125">Accept</span></span>|<span data-ttu-id="cbbf5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbbf5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbbf5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbbf5-127">Request body</span></span>
<span data-ttu-id="cbbf5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbbf5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cbbf5-129">Response</span></span>
<span data-ttu-id="cbbf5-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbbf5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cbbf5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbbf5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbbf5-132">Request</span></span>
<span data-ttu-id="cbbf5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbbf5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="cbbf5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cbbf5-134">Response</span></span>
<span data-ttu-id="cbbf5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cbbf5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
      "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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





