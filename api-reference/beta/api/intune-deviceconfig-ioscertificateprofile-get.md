---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56ae60e6e94fcd9710a7a4e4b9ec85a38b4de3b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936573"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="f99ad-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f99ad-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="f99ad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f99ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f99ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f99ad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f99ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f99ad-107">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f99ad-107">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f99ad-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f99ad-108">Prerequisites</span></span>
<span data-ttu-id="f99ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f99ad-111">Permission type</span></span>|<span data-ttu-id="f99ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f99ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f99ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f99ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f99ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f99ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f99ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f99ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f99ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99ad-116">Not supported.</span></span>|
|<span data-ttu-id="f99ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f99ad-117">Application</span></span>|<span data-ttu-id="f99ad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f99ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeEncryptionCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f99ad-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f99ad-120">Optional query parameters</span></span>
<span data-ttu-id="f99ad-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f99ad-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f99ad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f99ad-122">Request headers</span></span>
|<span data-ttu-id="f99ad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f99ad-123">Header</span></span>|<span data-ttu-id="f99ad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f99ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f99ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f99ad-125">Authorization</span></span>|<span data-ttu-id="f99ad-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f99ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f99ad-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f99ad-127">Accept</span></span>|<span data-ttu-id="f99ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f99ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f99ad-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f99ad-129">Request body</span></span>
<span data-ttu-id="f99ad-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f99ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f99ad-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f99ad-131">Response</span></span>
<span data-ttu-id="f99ad-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f99ad-132">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99ad-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f99ad-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f99ad-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f99ad-134">Request</span></span>
<span data-ttu-id="f99ad-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f99ad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="f99ad-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f99ad-136">Response</span></span>
<span data-ttu-id="f99ad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f99ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 464

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```





