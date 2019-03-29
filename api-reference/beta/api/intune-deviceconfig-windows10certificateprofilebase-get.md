---
title: Получение windows10CertificateProfileBase
description: Чтение свойств и связей объекта windows10CertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7a035564fac516d278933edbaac0ab91b63b50f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981169"
---
# <a name="get-windows10certificateprofilebase"></a><span data-ttu-id="763eb-103">Получение windows10CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="763eb-103">Get windows10CertificateProfileBase</span></span>

> <span data-ttu-id="763eb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="763eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="763eb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="763eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="763eb-106">Чтение свойств и связей объекта [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="763eb-106">Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="763eb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="763eb-107">Prerequisites</span></span>
<span data-ttu-id="763eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="763eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="763eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="763eb-110">Permission type</span></span>|<span data-ttu-id="763eb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="763eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="763eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="763eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="763eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="763eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="763eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="763eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="763eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="763eb-115">Not supported.</span></span>|
|<span data-ttu-id="763eb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="763eb-116">Application</span></span>|<span data-ttu-id="763eb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="763eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="763eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="763eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="763eb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="763eb-119">Optional query parameters</span></span>
<span data-ttu-id="763eb-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="763eb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="763eb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="763eb-121">Request headers</span></span>
|<span data-ttu-id="763eb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="763eb-122">Header</span></span>|<span data-ttu-id="763eb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="763eb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="763eb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="763eb-124">Authorization</span></span>|<span data-ttu-id="763eb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="763eb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="763eb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="763eb-126">Accept</span></span>|<span data-ttu-id="763eb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="763eb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="763eb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="763eb-128">Request body</span></span>
<span data-ttu-id="763eb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="763eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="763eb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="763eb-130">Response</span></span>
<span data-ttu-id="763eb-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="763eb-131">If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="763eb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="763eb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="763eb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="763eb-133">Request</span></span>
<span data-ttu-id="763eb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="763eb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="763eb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="763eb-135">Response</span></span>
<span data-ttu-id="763eb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="763eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CertificateProfileBase",
    "id": "1f01ffc6-ffc6-1f01-c6ff-011fc6ff011f",
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
    "certificateValidityPeriodScale": "months"
  }
}
```




