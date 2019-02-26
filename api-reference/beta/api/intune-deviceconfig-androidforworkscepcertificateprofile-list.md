---
title: Список Андроидфорворксцепцертификатепрофилес
description: Список свойств и связей объектов androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66bb2d49fe9a61c12d835cbf8928d4f45956792c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152866"
---
# <a name="list-androidforworkscepcertificateprofiles"></a><span data-ttu-id="c4f39-103">Список Андроидфорворксцепцертификатепрофилес</span><span class="sxs-lookup"><span data-stu-id="c4f39-103">List androidForWorkScepCertificateProfiles</span></span>

> <span data-ttu-id="c4f39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4f39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4f39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f39-106">Список свойств и связей объектов [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c4f39-106">List properties and relationships of the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4f39-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4f39-107">Prerequisites</span></span>
<span data-ttu-id="c4f39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4f39-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4f39-110">Permission type</span></span>|<span data-ttu-id="c4f39-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4f39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4f39-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4f39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4f39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c4f39-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4f39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4f39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f39-115">Not supported.</span></span>|
|<span data-ttu-id="c4f39-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4f39-116">Application</span></span>|<span data-ttu-id="c4f39-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4f39-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4f39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c4f39-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4f39-119">Request headers</span></span>
|<span data-ttu-id="c4f39-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4f39-120">Header</span></span>|<span data-ttu-id="c4f39-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4f39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4f39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4f39-122">Authorization</span></span>|<span data-ttu-id="c4f39-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c4f39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4f39-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c4f39-124">Accept</span></span>|<span data-ttu-id="c4f39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4f39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4f39-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4f39-126">Request body</span></span>
<span data-ttu-id="c4f39-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4f39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4f39-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4f39-128">Response</span></span>
<span data-ttu-id="c4f39-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4f39-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f39-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f39-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4f39-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4f39-131">Request</span></span>
<span data-ttu-id="c4f39-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4f39-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c4f39-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4f39-133">Response</span></span>
<span data-ttu-id="c4f39-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c4f39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




