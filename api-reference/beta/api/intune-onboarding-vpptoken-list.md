---
title: Список VPP токенов
description: Список свойств и связей объектов VPP токен.
author: tfitzmac
ms.openlocfilehash: 7a3e1d52c91d28b1714b1111f3207942355c5156
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344333"
---
# <a name="list-vpptokens"></a><span data-ttu-id="24ede-103">Список VPP токенов</span><span class="sxs-lookup"><span data-stu-id="24ede-103">List vppTokens</span></span>

> <span data-ttu-id="24ede-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24ede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24ede-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24ede-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="24ede-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24ede-107">Список свойств и связей объектов [VPP токены](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="24ede-107">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24ede-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="24ede-108">Prerequisites</span></span>
<span data-ttu-id="24ede-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24ede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24ede-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24ede-111">Permission type</span></span>|<span data-ttu-id="24ede-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24ede-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24ede-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24ede-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24ede-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24ede-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="24ede-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24ede-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24ede-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ede-116">Not supported.</span></span>|
|<span data-ttu-id="24ede-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24ede-117">Application</span></span>|<span data-ttu-id="24ede-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ede-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24ede-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24ede-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="24ede-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24ede-120">Request headers</span></span>
|<span data-ttu-id="24ede-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24ede-121">Header</span></span>|<span data-ttu-id="24ede-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24ede-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24ede-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24ede-123">Authorization</span></span>|<span data-ttu-id="24ede-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="24ede-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24ede-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24ede-125">Accept</span></span>|<span data-ttu-id="24ede-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24ede-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24ede-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24ede-127">Request body</span></span>
<span data-ttu-id="24ede-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24ede-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24ede-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="24ede-129">Response</span></span>
<span data-ttu-id="24ede-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [VPP Токенов ](../resources/intune-onboarding-vpptoken.md) в текстовом поле для отклика.</span><span class="sxs-lookup"><span data-stu-id="24ede-130">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24ede-131">Пример</span><span class="sxs-lookup"><span data-stu-id="24ede-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="24ede-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="24ede-132">Request</span></span>
<span data-ttu-id="24ede-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24ede-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="24ede-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="24ede-134">Response</span></span>
<span data-ttu-id="24ede-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="24ede-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1190

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "tokenActionResults": [
        {
          "@odata.type": "microsoft.graph.vppTokenActionResult",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ],
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value",
      "dataSharingConsentGranted": true,
      "displayName": "Display Name value",
      "locationName": "Location Name value",
      "claimTokenManagementFromExternalMdm": true
    }
  ]
}
```





