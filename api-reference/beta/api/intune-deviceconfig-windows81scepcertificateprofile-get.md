---
title: Получение windows81SCEPCertificateProfile
description: Чтение свойства и связи объекта windows81SCEPCertificateProfile.
author: tfitzmac
ms.openlocfilehash: bb2f627738b3ab0e86826979f75f0863855e2142
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316284"
---
# <a name="get-windows81scepcertificateprofile"></a><span data-ttu-id="b82fc-103">Получение windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b82fc-103">Get windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="b82fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b82fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b82fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b82fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b82fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b82fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b82fc-107">Чтение свойства и связи объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b82fc-107">Read properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b82fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b82fc-108">Prerequisites</span></span>
<span data-ttu-id="b82fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b82fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b82fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b82fc-111">Permission type</span></span>|<span data-ttu-id="b82fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b82fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b82fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b82fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b82fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b82fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b82fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b82fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b82fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b82fc-116">Not supported.</span></span>|
|<span data-ttu-id="b82fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b82fc-117">Application</span></span>|<span data-ttu-id="b82fc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b82fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b82fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b82fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b82fc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b82fc-120">Optional query parameters</span></span>
<span data-ttu-id="b82fc-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b82fc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b82fc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b82fc-122">Request headers</span></span>
|<span data-ttu-id="b82fc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b82fc-123">Header</span></span>|<span data-ttu-id="b82fc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b82fc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b82fc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b82fc-125">Authorization</span></span>|<span data-ttu-id="b82fc-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b82fc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b82fc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b82fc-127">Accept</span></span>|<span data-ttu-id="b82fc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b82fc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b82fc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b82fc-129">Request body</span></span>
<span data-ttu-id="b82fc-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b82fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b82fc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b82fc-131">Response</span></span>
<span data-ttu-id="b82fc-132">Успешно завершена, этот метод возвращает `200 OK` объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b82fc-132">If successful, this method returns a `200 OK` response code and [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b82fc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b82fc-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b82fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b82fc-134">Request</span></span>
<span data-ttu-id="b82fc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b82fc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b82fc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b82fc-136">Response</span></span>
<span data-ttu-id="b82fc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b82fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1522

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
    "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "customSubjectAlternativeNames": [
      {
        "@odata.type": "microsoft.graph.customSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ],
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "certificateStore": "machine"
  }
}
```





