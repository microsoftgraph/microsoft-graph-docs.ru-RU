---
title: Список windowsCertificateProfileBases
description: Свойства списка и связей объектов windowsCertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 770a17633b531c63e9defea6f3858b137e5155b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886284"
---
# <a name="list-windowscertificateprofilebases"></a><span data-ttu-id="36241-103">Список windowsCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="36241-103">List windowsCertificateProfileBases</span></span>

> <span data-ttu-id="36241-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36241-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36241-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36241-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36241-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36241-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36241-107">Свойства списка и связей объектов [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="36241-107">List properties and relationships of the [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36241-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36241-108">Prerequisites</span></span>
<span data-ttu-id="36241-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36241-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36241-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36241-111">Permission type</span></span>|<span data-ttu-id="36241-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36241-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36241-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36241-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36241-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36241-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36241-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36241-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36241-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36241-116">Not supported.</span></span>|
|<span data-ttu-id="36241-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36241-117">Application</span></span>|<span data-ttu-id="36241-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36241-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36241-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36241-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36241-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36241-120">Request headers</span></span>
|<span data-ttu-id="36241-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36241-121">Header</span></span>|<span data-ttu-id="36241-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36241-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36241-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36241-123">Authorization</span></span>|<span data-ttu-id="36241-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36241-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36241-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36241-125">Accept</span></span>|<span data-ttu-id="36241-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36241-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36241-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36241-127">Request body</span></span>
<span data-ttu-id="36241-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36241-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36241-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="36241-129">Response</span></span>
<span data-ttu-id="36241-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36241-130">If successful, this method returns a `200 OK` response code and a collection of [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36241-131">Пример</span><span class="sxs-lookup"><span data-stu-id="36241-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36241-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="36241-132">Request</span></span>
<span data-ttu-id="36241-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36241-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="36241-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="36241-134">Response</span></span>
<span data-ttu-id="36241-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="36241-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsCertificateProfileBase",
      "id": "c0979ce1-9ce1-c097-e19c-97c0e19c97c0",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





