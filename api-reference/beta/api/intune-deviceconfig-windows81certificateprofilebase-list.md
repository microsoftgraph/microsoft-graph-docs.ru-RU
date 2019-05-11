---
title: Список windows81CertificateProfileBases
description: Список свойств и связей объектов windows81CertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a821364c8a27739ff6d94d91d32c6a7880bea91
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918341"
---
# <a name="list-windows81certificateprofilebases"></a><span data-ttu-id="caaeb-103">Список windows81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="caaeb-103">List windows81CertificateProfileBases</span></span>

> <span data-ttu-id="caaeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caaeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caaeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="caaeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caaeb-106">Список свойств и связей объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="caaeb-106">List properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caaeb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="caaeb-107">Prerequisites</span></span>
<span data-ttu-id="caaeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caaeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caaeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caaeb-110">Permission type</span></span>|<span data-ttu-id="caaeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="caaeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caaeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caaeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="caaeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="caaeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="caaeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caaeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caaeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caaeb-115">Not supported.</span></span>|
|<span data-ttu-id="caaeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caaeb-116">Application</span></span>|<span data-ttu-id="caaeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caaeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caaeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caaeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="caaeb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caaeb-119">Request headers</span></span>
|<span data-ttu-id="caaeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caaeb-120">Header</span></span>|<span data-ttu-id="caaeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="caaeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caaeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="caaeb-122">Authorization</span></span>|<span data-ttu-id="caaeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caaeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caaeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="caaeb-124">Accept</span></span>|<span data-ttu-id="caaeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="caaeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caaeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="caaeb-126">Request body</span></span>
<span data-ttu-id="caaeb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="caaeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caaeb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="caaeb-128">Response</span></span>
<span data-ttu-id="caaeb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="caaeb-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caaeb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="caaeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="caaeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="caaeb-131">Request</span></span>
<span data-ttu-id="caaeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caaeb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="caaeb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="caaeb-133">Response</span></span>
<span data-ttu-id="caaeb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="caaeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
      "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
      ]
    }
  ]
}
```




