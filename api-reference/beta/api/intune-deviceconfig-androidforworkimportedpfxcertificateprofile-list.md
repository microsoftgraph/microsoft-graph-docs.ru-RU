---
title: Список androidForWorkImportedPFXCertificateProfiles
description: Свойства списка и связей объектов androidForWorkImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2c86bb8cabecf19278d94807f672c195178bbc8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412956"
---
# <a name="list-androidforworkimportedpfxcertificateprofiles"></a><span data-ttu-id="181fb-103">Список androidForWorkImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="181fb-103">List androidForWorkImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="181fb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="181fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="181fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="181fb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="181fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="181fb-107">Свойства списка и связей объектов [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="181fb-107">List properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="181fb-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="181fb-108">Prerequisites</span></span>
<span data-ttu-id="181fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="181fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="181fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="181fb-111">Permission type</span></span>|<span data-ttu-id="181fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="181fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="181fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="181fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="181fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="181fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="181fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="181fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="181fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181fb-116">Not supported.</span></span>|
|<span data-ttu-id="181fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="181fb-117">Application</span></span>|<span data-ttu-id="181fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="181fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="181fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="181fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="181fb-120">Request headers</span></span>
|<span data-ttu-id="181fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="181fb-121">Header</span></span>|<span data-ttu-id="181fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="181fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="181fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="181fb-123">Authorization</span></span>|<span data-ttu-id="181fb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="181fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="181fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="181fb-125">Accept</span></span>|<span data-ttu-id="181fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="181fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="181fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="181fb-127">Request body</span></span>
<span data-ttu-id="181fb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="181fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181fb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="181fb-129">Response</span></span>
<span data-ttu-id="181fb-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="181fb-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181fb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="181fb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="181fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="181fb-132">Request</span></span>
<span data-ttu-id="181fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="181fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="181fb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="181fb-134">Response</span></span>
<span data-ttu-id="181fb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="181fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
      "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




