---
title: Список Интунебрандингпрофилес
description: Список свойств и связей объектов Интунебрандингпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f49bd126bbcb6d362d804007bacf6c7c7b4f265
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970711"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="e3a93-103">Список Интунебрандингпрофилес</span><span class="sxs-lookup"><span data-stu-id="e3a93-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="e3a93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3a93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3a93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3a93-106">Список свойств и связей объектов [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e3a93-106">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3a93-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3a93-107">Prerequisites</span></span>
<span data-ttu-id="e3a93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3a93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a93-110">Permission type</span></span>|<span data-ttu-id="e3a93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3a93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3a93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3a93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3a93-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3a93-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3a93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3a93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3a93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a93-115">Not supported.</span></span>|
|<span data-ttu-id="e3a93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3a93-116">Application</span></span>|<span data-ttu-id="e3a93-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a93-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3a93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3a93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e3a93-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3a93-119">Request headers</span></span>
|<span data-ttu-id="e3a93-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3a93-120">Header</span></span>|<span data-ttu-id="e3a93-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e3a93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3a93-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3a93-122">Authorization</span></span>|<span data-ttu-id="e3a93-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3a93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3a93-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e3a93-124">Accept</span></span>|<span data-ttu-id="e3a93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3a93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3a93-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3a93-126">Request body</span></span>
<span data-ttu-id="e3a93-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3a93-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3a93-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a93-128">Response</span></span>
<span data-ttu-id="e3a93-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a93-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3a93-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e3a93-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3a93-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a93-131">Request</span></span>
<span data-ttu-id="e3a93-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3a93-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="e3a93-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3a93-133">Response</span></span>
<span data-ttu-id="e3a93-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3a93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

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
      "contactITName": "Contact ITName value",
      "contactITPhoneNumber": "Contact ITPhone Number value",
      "contactITEmailAddress": "Contact ITEmail Address value",
      "contactITNotes": "Contact ITNotes value",
      "privacyUrl": "https://example.com/privacyUrl/",
      "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
      "onlineSupportSiteName": "Online Support Site Name value",
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
      }
    }
  ]
}
```




