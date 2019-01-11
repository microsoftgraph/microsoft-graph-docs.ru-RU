---
title: Получение iosPkcsCertificateProfile
description: Чтение свойства и связи объекта iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81e09211a9e98e27b4456a6f3bc0e19c55e1b4fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878437"
---
# <a name="get-iospkcscertificateprofile"></a><span data-ttu-id="35164-103">Получение iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="35164-103">Get iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="35164-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35164-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35164-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35164-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35164-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35164-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35164-107">Чтение свойства и связи объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="35164-107">Read properties and relationships of the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35164-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35164-108">Prerequisites</span></span>
<span data-ttu-id="35164-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35164-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35164-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35164-111">Permission type</span></span>|<span data-ttu-id="35164-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35164-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35164-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35164-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35164-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35164-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35164-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35164-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35164-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35164-116">Not supported.</span></span>|
|<span data-ttu-id="35164-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35164-117">Application</span></span>|<span data-ttu-id="35164-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35164-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35164-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35164-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35164-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35164-120">Optional query parameters</span></span>
<span data-ttu-id="35164-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35164-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35164-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35164-122">Request headers</span></span>
|<span data-ttu-id="35164-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35164-123">Header</span></span>|<span data-ttu-id="35164-124">Значение</span><span class="sxs-lookup"><span data-stu-id="35164-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35164-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="35164-125">Authorization</span></span>|<span data-ttu-id="35164-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35164-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35164-127">Accept</span><span class="sxs-lookup"><span data-stu-id="35164-127">Accept</span></span>|<span data-ttu-id="35164-128">application/json</span><span class="sxs-lookup"><span data-stu-id="35164-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35164-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35164-129">Request body</span></span>
<span data-ttu-id="35164-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35164-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35164-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="35164-131">Response</span></span>
<span data-ttu-id="35164-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="35164-132">If successful, this method returns a `200 OK` response code and [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35164-133">Пример</span><span class="sxs-lookup"><span data-stu-id="35164-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="35164-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="35164-134">Request</span></span>
<span data-ttu-id="35164-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35164-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="35164-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="35164-136">Response</span></span>
<span data-ttu-id="35164-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35164-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 992

{
  "value": {
    "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
    "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
    "subjectNameFormat": "commonNameAsEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```





