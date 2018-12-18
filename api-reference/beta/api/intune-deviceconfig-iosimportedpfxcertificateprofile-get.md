---
title: Получение iosImportedPFXCertificateProfile
description: Чтение свойства и связи объекта iosImportedPFXCertificateProfile.
author: tfitzmac
ms.openlocfilehash: d12dfdad92a672d4515ae6190d6ce5de73845b3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350870"
---
# <a name="get-iosimportedpfxcertificateprofile"></a><span data-ttu-id="d11ec-103">Получение iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d11ec-103">Get iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d11ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d11ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d11ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d11ec-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d11ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d11ec-107">Чтение свойства и связи объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d11ec-107">Read properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d11ec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d11ec-108">Prerequisites</span></span>
<span data-ttu-id="d11ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11ec-111">Permission type</span></span>|<span data-ttu-id="d11ec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d11ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d11ec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d11ec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d11ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d11ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11ec-116">Not supported.</span></span>|
|<span data-ttu-id="d11ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d11ec-117">Application</span></span>|<span data-ttu-id="d11ec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d11ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d11ec-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d11ec-120">Optional query parameters</span></span>
<span data-ttu-id="d11ec-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d11ec-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d11ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d11ec-122">Request headers</span></span>
|<span data-ttu-id="d11ec-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d11ec-123">Header</span></span>|<span data-ttu-id="d11ec-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d11ec-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d11ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d11ec-125">Authorization</span></span>|<span data-ttu-id="d11ec-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d11ec-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d11ec-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d11ec-127">Accept</span></span>|<span data-ttu-id="d11ec-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d11ec-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d11ec-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11ec-129">Request body</span></span>
<span data-ttu-id="d11ec-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d11ec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d11ec-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d11ec-131">Response</span></span>
<span data-ttu-id="d11ec-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d11ec-132">If successful, this method returns a `200 OK` response code and [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d11ec-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d11ec-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d11ec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11ec-134">Request</span></span>
<span data-ttu-id="d11ec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d11ec-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d11ec-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d11ec-136">Response</span></span>
<span data-ttu-id="d11ec-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d11ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





