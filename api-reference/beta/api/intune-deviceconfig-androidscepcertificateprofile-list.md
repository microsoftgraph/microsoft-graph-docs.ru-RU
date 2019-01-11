---
title: Список androidScepCertificateProfiles
description: Свойства списка и связей объектов androidScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e34c772cc1b9bdcbe72d11280f5a5868106698e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852482"
---
# <a name="list-androidscepcertificateprofiles"></a><span data-ttu-id="a95e2-103">Список androidScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="a95e2-103">List androidScepCertificateProfiles</span></span>

> <span data-ttu-id="a95e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a95e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a95e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a95e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a95e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a95e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a95e2-107">Свойства списка и связей объектов [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a95e2-107">List properties and relationships of the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a95e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a95e2-108">Prerequisites</span></span>
<span data-ttu-id="a95e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a95e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a95e2-111">Permission type</span></span>|<span data-ttu-id="a95e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a95e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a95e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a95e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a95e2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a95e2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a95e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a95e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a95e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a95e2-116">Not supported.</span></span>|
|<span data-ttu-id="a95e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a95e2-117">Application</span></span>|<span data-ttu-id="a95e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a95e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a95e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a95e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a95e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a95e2-120">Request headers</span></span>
|<span data-ttu-id="a95e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a95e2-121">Header</span></span>|<span data-ttu-id="a95e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a95e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a95e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a95e2-123">Authorization</span></span>|<span data-ttu-id="a95e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a95e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a95e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a95e2-125">Accept</span></span>|<span data-ttu-id="a95e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a95e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a95e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a95e2-127">Request body</span></span>
<span data-ttu-id="a95e2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a95e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a95e2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a95e2-129">Response</span></span>
<span data-ttu-id="a95e2-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a95e2-130">If successful, this method returns a `200 OK` response code and a collection of [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a95e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a95e2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a95e2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a95e2-132">Request</span></span>
<span data-ttu-id="a95e2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a95e2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a95e2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a95e2-134">Response</span></span>
<span data-ttu-id="a95e2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a95e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
      "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```





