---
title: Список Интунебрандингпрофилес
description: Список свойств и связей объектов Интунебрандингпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccb19df24874b5d6c8bee245179bb26b0978559d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709049"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="4398b-103">Список Интунебрандингпрофилес</span><span class="sxs-lookup"><span data-stu-id="4398b-103">List intuneBrandingProfiles</span></span>

<span data-ttu-id="4398b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4398b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4398b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4398b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4398b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4398b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4398b-107">Список свойств и связей объектов [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4398b-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4398b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4398b-108">Prerequisites</span></span>
<span data-ttu-id="4398b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4398b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4398b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4398b-111">Permission type</span></span>|<span data-ttu-id="4398b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4398b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4398b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4398b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4398b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4398b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4398b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4398b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4398b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4398b-116">Not supported.</span></span>|
|<span data-ttu-id="4398b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4398b-117">Application</span></span>|<span data-ttu-id="4398b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4398b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4398b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4398b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4398b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4398b-120">Request headers</span></span>
|<span data-ttu-id="4398b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4398b-121">Header</span></span>|<span data-ttu-id="4398b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4398b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4398b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4398b-123">Authorization</span></span>|<span data-ttu-id="4398b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4398b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4398b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4398b-125">Accept</span></span>|<span data-ttu-id="4398b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4398b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4398b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4398b-127">Request body</span></span>
<span data-ttu-id="4398b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4398b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4398b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4398b-129">Response</span></span>
<span data-ttu-id="4398b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4398b-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4398b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4398b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4398b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4398b-132">Request</span></span>
<span data-ttu-id="4398b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4398b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="4398b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4398b-134">Response</span></span>
<span data-ttu-id="4398b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4398b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfile",
      "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
      "profileName": "Profile Name value",
      "profileDescription": "Profile Description value",
      "isDefaultProfile": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "themeColor": {
        "@odata.type": "microsoft.graph.rgbColor",
        "r": 1,
        "g": 1,
        "b": 1
      },
      "showLogo": true,
      "showDisplayNameNextToLogo": true,
      "themeColorLogo": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "lightBackgroundLogo": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "landingPageCustomizedImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "contactITName": "Contact ITName value",
      "contactITPhoneNumber": "Contact ITPhone Number value",
      "contactITEmailAddress": "Contact ITEmail Address value",
      "contactITNotes": "Contact ITNotes value",
      "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
      "onlineSupportSiteName": "Online Support Site Name value",
      "privacyUrl": "https://example.com/privacyUrl/",
      "customPrivacyMessage": "Custom Privacy Message value",
      "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
      "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
      "isRemoveDeviceDisabled": true,
      "isFactoryResetDisabled": true,
      "companyPortalBlockedActions": [
        {
          "@odata.type": "microsoft.graph.companyPortalBlockedAction",
          "platform": "androidForWork",
          "ownerType": "company",
          "action": "remove"
        }
      ],
      "showAzureADEnterpriseApps": true,
      "showOfficeWebApps": true,
      "sendDeviceOwnershipChangePushNotification": true,
      "enrollmentAvailability": "availableWithoutPrompts",
      "disableClientTelemetry": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





