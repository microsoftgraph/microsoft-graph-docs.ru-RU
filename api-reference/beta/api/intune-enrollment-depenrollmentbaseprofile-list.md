---
title: Список depEnrollmentBaseProfiles
description: Свойства списка и связей объектов depEnrollmentBaseProfile.
author: tfitzmac
ms.openlocfilehash: ce7edb9558864323ca08a4379ae0e6e8949c6875
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340959"
---
# <a name="list-depenrollmentbaseprofiles"></a><span data-ttu-id="f0daa-103">Список depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="f0daa-103">List depEnrollmentBaseProfiles</span></span>

> <span data-ttu-id="f0daa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0daa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0daa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0daa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0daa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0daa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0daa-107">Свойства списка и связей объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f0daa-107">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0daa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0daa-108">Prerequisites</span></span>
<span data-ttu-id="f0daa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0daa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0daa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0daa-111">Permission type</span></span>|<span data-ttu-id="f0daa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0daa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0daa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0daa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0daa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0daa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f0daa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0daa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0daa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0daa-116">Not supported.</span></span>|
|<span data-ttu-id="f0daa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0daa-117">Application</span></span>|<span data-ttu-id="f0daa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0daa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0daa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0daa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f0daa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0daa-120">Request headers</span></span>
|<span data-ttu-id="f0daa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0daa-121">Header</span></span>|<span data-ttu-id="f0daa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0daa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0daa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0daa-123">Authorization</span></span>|<span data-ttu-id="f0daa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0daa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0daa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0daa-125">Accept</span></span>|<span data-ttu-id="f0daa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0daa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0daa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0daa-127">Request body</span></span>
<span data-ttu-id="f0daa-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0daa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0daa-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0daa-129">Response</span></span>
<span data-ttu-id="f0daa-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f0daa-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0daa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f0daa-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0daa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0daa-132">Request</span></span>
<span data-ttu-id="f0daa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0daa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="f0daa-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0daa-134">Response</span></span>
<span data-ttu-id="f0daa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0daa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
      "id": "db378868-8868-db37-6888-37db688837db",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true
    }
  ]
}
```





