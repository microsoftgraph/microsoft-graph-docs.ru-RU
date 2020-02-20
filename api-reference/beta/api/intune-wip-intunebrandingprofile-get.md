---
title: Получение Интунебрандингпрофиле
description: Чтение свойств и связей объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d228cd67506c4c4ae968c255ee26d259542d4091
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161525"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="4d4d3-103">Получение Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="4d4d3-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="4d4d3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d4d3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d4d3-106">Чтение свойств и связей объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4d4d3-106">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d4d3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d4d3-107">Prerequisites</span></span>
<span data-ttu-id="4d4d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d4d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d4d3-110">Permission type</span></span>|<span data-ttu-id="4d4d3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d4d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d4d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d4d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d4d3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4d3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d4d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d4d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d4d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-115">Not supported.</span></span>|
|<span data-ttu-id="4d4d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d4d3-116">Application</span></span>|<span data-ttu-id="4d4d3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4d3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d4d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d4d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d4d3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d4d3-119">Optional query parameters</span></span>
<span data-ttu-id="4d4d3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d4d3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d4d3-121">Request headers</span></span>
|<span data-ttu-id="4d4d3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d4d3-122">Header</span></span>|<span data-ttu-id="4d4d3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4d4d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d4d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d4d3-124">Authorization</span></span>|<span data-ttu-id="4d4d3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d4d3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4d4d3-126">Accept</span></span>|<span data-ttu-id="4d4d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4d4d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d4d3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d4d3-128">Request body</span></span>
<span data-ttu-id="4d4d3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d4d3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d4d3-130">Response</span></span>
<span data-ttu-id="4d4d3-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d4d3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4d4d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d4d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d4d3-133">Request</span></span>
<span data-ttu-id="4d4d3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="4d4d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d4d3-135">Response</span></span>
<span data-ttu-id="4d4d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d4d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





