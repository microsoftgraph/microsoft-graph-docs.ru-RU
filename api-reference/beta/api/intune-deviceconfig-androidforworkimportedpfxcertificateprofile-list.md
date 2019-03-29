---
title: Список Андроидфорворкимпортедпфксцертификатепрофилес
description: Список свойств и связей объектов Андроидфорворкимпортедпфксцертификатепрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05eac6207534419ad2ae4c34927f1074ed43b248
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956739"
---
# <a name="list-androidforworkimportedpfxcertificateprofiles"></a><span data-ttu-id="aca98-103">Список Андроидфорворкимпортедпфксцертификатепрофилес</span><span class="sxs-lookup"><span data-stu-id="aca98-103">List androidForWorkImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="aca98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aca98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aca98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aca98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aca98-106">Список свойств и связей объектов [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aca98-106">List properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aca98-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aca98-107">Prerequisites</span></span>
<span data-ttu-id="aca98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aca98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aca98-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aca98-110">Permission type</span></span>|<span data-ttu-id="aca98-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aca98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aca98-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aca98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aca98-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca98-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aca98-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aca98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aca98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aca98-115">Not supported.</span></span>|
|<span data-ttu-id="aca98-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aca98-116">Application</span></span>|<span data-ttu-id="aca98-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aca98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aca98-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aca98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aca98-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aca98-119">Request headers</span></span>
|<span data-ttu-id="aca98-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aca98-120">Header</span></span>|<span data-ttu-id="aca98-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aca98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aca98-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aca98-122">Authorization</span></span>|<span data-ttu-id="aca98-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aca98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aca98-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aca98-124">Accept</span></span>|<span data-ttu-id="aca98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aca98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aca98-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aca98-126">Request body</span></span>
<span data-ttu-id="aca98-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aca98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aca98-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="aca98-128">Response</span></span>
<span data-ttu-id="aca98-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aca98-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aca98-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aca98-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aca98-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aca98-131">Request</span></span>
<span data-ttu-id="aca98-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aca98-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="aca98-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aca98-133">Response</span></span>
<span data-ttu-id="aca98-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aca98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




