---
title: Получение Иосимпортедпфксцертификатепрофиле
description: Чтение свойств и связей объекта Иосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15612b205dae24f739f7d42b0d906bef03e3e1c0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923407"
---
# <a name="get-iosimportedpfxcertificateprofile"></a><span data-ttu-id="7dd38-103">Получение Иосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="7dd38-103">Get iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="7dd38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dd38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dd38-106">Чтение свойств и связей объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7dd38-106">Read properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dd38-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7dd38-107">Prerequisites</span></span>
<span data-ttu-id="7dd38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dd38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd38-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd38-110">Permission type</span></span>|<span data-ttu-id="7dd38-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dd38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dd38-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dd38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dd38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dd38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7dd38-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dd38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dd38-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd38-115">Not supported.</span></span>|
|<span data-ttu-id="7dd38-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dd38-116">Application</span></span>|<span data-ttu-id="7dd38-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dd38-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dd38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dd38-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7dd38-119">Optional query parameters</span></span>
<span data-ttu-id="7dd38-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7dd38-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dd38-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dd38-121">Request headers</span></span>
|<span data-ttu-id="7dd38-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dd38-122">Header</span></span>|<span data-ttu-id="7dd38-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7dd38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dd38-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dd38-124">Authorization</span></span>|<span data-ttu-id="7dd38-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dd38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dd38-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7dd38-126">Accept</span></span>|<span data-ttu-id="7dd38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7dd38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dd38-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dd38-128">Request body</span></span>
<span data-ttu-id="7dd38-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dd38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dd38-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dd38-130">Response</span></span>
<span data-ttu-id="7dd38-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd38-131">If successful, this method returns a `200 OK` response code and [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7dd38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dd38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd38-133">Request</span></span>
<span data-ttu-id="7dd38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd38-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7dd38-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd38-135">Response</span></span>
<span data-ttu-id="7dd38-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": {
    "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
    "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "intendedPurpose": "smimeEncryption"
  }
}
```




