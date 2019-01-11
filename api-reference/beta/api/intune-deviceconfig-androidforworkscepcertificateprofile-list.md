---
title: Список androidForWorkScepCertificateProfiles
description: Свойства списка и связей объектов androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 426e4c390133214132efe5c167a0adcd96c81306
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878115"
---
# <a name="list-androidforworkscepcertificateprofiles"></a><span data-ttu-id="1b9d2-103">Список androidForWorkScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="1b9d2-103">List androidForWorkScepCertificateProfiles</span></span>

> <span data-ttu-id="1b9d2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b9d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b9d2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b9d2-107">Свойства списка и связей объектов [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1b9d2-107">List properties and relationships of the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b9d2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b9d2-108">Prerequisites</span></span>
<span data-ttu-id="1b9d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b9d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b9d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b9d2-111">Permission type</span></span>|<span data-ttu-id="1b9d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b9d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b9d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b9d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b9d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b9d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1b9d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b9d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b9d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-116">Not supported.</span></span>|
|<span data-ttu-id="1b9d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b9d2-117">Application</span></span>|<span data-ttu-id="1b9d2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b9d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b9d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b9d2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b9d2-120">Request headers</span></span>
|<span data-ttu-id="1b9d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b9d2-121">Header</span></span>|<span data-ttu-id="1b9d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b9d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b9d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b9d2-123">Authorization</span></span>|<span data-ttu-id="1b9d2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b9d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b9d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b9d2-125">Accept</span></span>|<span data-ttu-id="1b9d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b9d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b9d2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b9d2-127">Request body</span></span>
<span data-ttu-id="1b9d2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b9d2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b9d2-129">Response</span></span>
<span data-ttu-id="1b9d2-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b9d2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1b9d2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b9d2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b9d2-132">Request</span></span>
<span data-ttu-id="1b9d2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1b9d2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b9d2-134">Response</span></span>
<span data-ttu-id="1b9d2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b9d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1566

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
      "id": "09e532af-32af-09e5-af32-e509af32e509",
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
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
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
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```





