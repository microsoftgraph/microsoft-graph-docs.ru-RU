---
title: Получение androidCertificateProfileBase
description: Чтение свойства и связи объекта androidCertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd8dc677d0c388c8f5c6bc9763855daf8fb90a22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822822"
---
# <a name="get-androidcertificateprofilebase"></a><span data-ttu-id="a0c48-103">Получение androidCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="a0c48-103">Get androidCertificateProfileBase</span></span>

> <span data-ttu-id="a0c48-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0c48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0c48-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0c48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0c48-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0c48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0c48-107">Чтение свойства и связи объекта [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c48-107">Read properties and relationships of the [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0c48-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0c48-108">Prerequisites</span></span>
<span data-ttu-id="a0c48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0c48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0c48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0c48-111">Permission type</span></span>|<span data-ttu-id="a0c48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0c48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0c48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0c48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0c48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0c48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0c48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0c48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0c48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0c48-116">Not supported.</span></span>|
|<span data-ttu-id="a0c48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0c48-117">Application</span></span>|<span data-ttu-id="a0c48-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0c48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0c48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0c48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0c48-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0c48-120">Optional query parameters</span></span>
<span data-ttu-id="a0c48-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0c48-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0c48-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0c48-122">Request headers</span></span>
|<span data-ttu-id="a0c48-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0c48-123">Header</span></span>|<span data-ttu-id="a0c48-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a0c48-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0c48-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0c48-125">Authorization</span></span>|<span data-ttu-id="a0c48-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a0c48-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0c48-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a0c48-127">Accept</span></span>|<span data-ttu-id="a0c48-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a0c48-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0c48-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0c48-129">Request body</span></span>
<span data-ttu-id="a0c48-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0c48-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0c48-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0c48-131">Response</span></span>
<span data-ttu-id="a0c48-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0c48-132">If successful, this method returns a `200 OK` response code and [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0c48-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a0c48-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0c48-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0c48-134">Request</span></span>
<span data-ttu-id="a0c48-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0c48-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="a0c48-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0c48-136">Response</span></span>
<span data-ttu-id="a0c48-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a0c48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCertificateProfileBase",
    "id": "76cf241d-241d-76cf-1d24-cf761d24cf76",
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
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ]
  }
}
```





