---
title: Получение iosImportedPFXCertificateProfile
description: Чтение свойства и связи объекта iosImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 92d1b28e2c3d0acd3ddfd0ed236674671c03fa6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398466"
---
# <a name="get-iosimportedpfxcertificateprofile"></a><span data-ttu-id="9eaca-103">Получение iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9eaca-103">Get iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="9eaca-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9eaca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9eaca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eaca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9eaca-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9eaca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eaca-107">Чтение свойства и связи объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9eaca-107">Read properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9eaca-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9eaca-108">Prerequisites</span></span>
<span data-ttu-id="9eaca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9eaca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9eaca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9eaca-111">Permission type</span></span>|<span data-ttu-id="9eaca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9eaca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eaca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9eaca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9eaca-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9eaca-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9eaca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9eaca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eaca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eaca-116">Not supported.</span></span>|
|<span data-ttu-id="9eaca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9eaca-117">Application</span></span>|<span data-ttu-id="9eaca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eaca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eaca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9eaca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9eaca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9eaca-120">Optional query parameters</span></span>
<span data-ttu-id="9eaca-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9eaca-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eaca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9eaca-122">Request headers</span></span>
|<span data-ttu-id="9eaca-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9eaca-123">Header</span></span>|<span data-ttu-id="9eaca-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9eaca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eaca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eaca-125">Authorization</span></span>|<span data-ttu-id="9eaca-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9eaca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eaca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9eaca-127">Accept</span></span>|<span data-ttu-id="9eaca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9eaca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eaca-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9eaca-129">Request body</span></span>
<span data-ttu-id="9eaca-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9eaca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eaca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eaca-131">Response</span></span>
<span data-ttu-id="9eaca-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9eaca-132">If successful, this method returns a `200 OK` response code and [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eaca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9eaca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9eaca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9eaca-134">Request</span></span>
<span data-ttu-id="9eaca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9eaca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9eaca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eaca-136">Response</span></span>
<span data-ttu-id="9eaca-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9eaca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




