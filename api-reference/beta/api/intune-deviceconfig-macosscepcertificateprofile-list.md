---
title: Список macOSScepCertificateProfiles
description: Свойства списка и связей объектов macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a72c172852b57de2ad92b4f017006257886df2fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983039"
---
# <a name="list-macosscepcertificateprofiles"></a><span data-ttu-id="ed98b-103">Список macOSScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="ed98b-103">List macOSScepCertificateProfiles</span></span>

> <span data-ttu-id="ed98b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed98b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed98b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed98b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed98b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed98b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed98b-107">Свойства списка и связей объектов [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ed98b-107">List properties and relationships of the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed98b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed98b-108">Prerequisites</span></span>
<span data-ttu-id="ed98b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed98b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed98b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed98b-111">Permission type</span></span>|<span data-ttu-id="ed98b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed98b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed98b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed98b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed98b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed98b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ed98b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed98b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed98b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed98b-116">Not supported.</span></span>|
|<span data-ttu-id="ed98b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed98b-117">Application</span></span>|<span data-ttu-id="ed98b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed98b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed98b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed98b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ed98b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed98b-120">Request headers</span></span>
|<span data-ttu-id="ed98b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed98b-121">Header</span></span>|<span data-ttu-id="ed98b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ed98b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed98b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed98b-123">Authorization</span></span>|<span data-ttu-id="ed98b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed98b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed98b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed98b-125">Accept</span></span>|<span data-ttu-id="ed98b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed98b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed98b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed98b-127">Request body</span></span>
<span data-ttu-id="ed98b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed98b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed98b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed98b-129">Response</span></span>
<span data-ttu-id="ed98b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ed98b-130">If successful, this method returns a `200 OK` response code and a collection of [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed98b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ed98b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed98b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed98b-132">Request</span></span>
<span data-ttu-id="ed98b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed98b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ed98b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed98b-134">Response</span></span>
<span data-ttu-id="ed98b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed98b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
      "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```





