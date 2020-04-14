---
title: Получение Интунебрандингпрофиле
description: Чтение свойств и связей объекта Интунебрандингпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2915b03d1dc850ee854f0b696a54efe109fd60c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458173"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="10daa-103">Получение Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10daa-103">Get intuneBrandingProfile</span></span>

<span data-ttu-id="10daa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10daa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10daa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10daa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10daa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10daa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10daa-107">Чтение свойств и связей объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="10daa-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10daa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10daa-108">Prerequisites</span></span>
<span data-ttu-id="10daa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10daa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10daa-111">Permission type</span></span>|<span data-ttu-id="10daa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10daa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10daa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10daa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10daa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10daa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10daa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10daa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10daa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10daa-116">Not supported.</span></span>|
|<span data-ttu-id="10daa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10daa-117">Application</span></span>|<span data-ttu-id="10daa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10daa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10daa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10daa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10daa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10daa-120">Optional query parameters</span></span>
<span data-ttu-id="10daa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10daa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10daa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10daa-122">Request headers</span></span>
|<span data-ttu-id="10daa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10daa-123">Header</span></span>|<span data-ttu-id="10daa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="10daa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10daa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10daa-125">Authorization</span></span>|<span data-ttu-id="10daa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10daa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10daa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="10daa-127">Accept</span></span>|<span data-ttu-id="10daa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10daa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10daa-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10daa-129">Request body</span></span>
<span data-ttu-id="10daa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10daa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10daa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="10daa-131">Response</span></span>
<span data-ttu-id="10daa-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10daa-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10daa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="10daa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="10daa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="10daa-134">Request</span></span>
<span data-ttu-id="10daa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10daa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="10daa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="10daa-136">Response</span></span>
<span data-ttu-id="10daa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10daa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2095

{
  "value": {
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
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```



