---
title: Получение windows10CertificateProfileBase
description: Чтение свойства и связи объекта windows10CertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e9596cc1cfacd89435394f5db62bf1a2a3e3e87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984404"
---
# <a name="get-windows10certificateprofilebase"></a><span data-ttu-id="bc250-103">Получение windows10CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="bc250-103">Get windows10CertificateProfileBase</span></span>

> <span data-ttu-id="bc250-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc250-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc250-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc250-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc250-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc250-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc250-107">Чтение свойства и связи объекта [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="bc250-107">Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc250-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc250-108">Prerequisites</span></span>
<span data-ttu-id="bc250-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc250-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc250-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc250-111">Permission type</span></span>|<span data-ttu-id="bc250-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc250-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc250-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc250-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc250-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc250-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc250-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc250-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc250-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc250-116">Not supported.</span></span>|
|<span data-ttu-id="bc250-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc250-117">Application</span></span>|<span data-ttu-id="bc250-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc250-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc250-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc250-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc250-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc250-120">Optional query parameters</span></span>
<span data-ttu-id="bc250-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc250-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc250-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc250-122">Request headers</span></span>
|<span data-ttu-id="bc250-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc250-123">Header</span></span>|<span data-ttu-id="bc250-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bc250-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc250-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc250-125">Authorization</span></span>|<span data-ttu-id="bc250-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc250-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc250-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bc250-127">Accept</span></span>|<span data-ttu-id="bc250-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bc250-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc250-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc250-129">Request body</span></span>
<span data-ttu-id="bc250-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc250-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc250-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc250-131">Response</span></span>
<span data-ttu-id="bc250-132">Успешно завершена, этот метод возвращает `200 OK` объект [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc250-132">If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc250-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bc250-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc250-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc250-134">Request</span></span>
<span data-ttu-id="bc250-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc250-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bc250-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc250-136">Response</span></span>
<span data-ttu-id="bc250-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc250-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





