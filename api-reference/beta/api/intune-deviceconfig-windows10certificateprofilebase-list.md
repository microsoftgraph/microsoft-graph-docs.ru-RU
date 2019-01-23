---
title: Список windows10CertificateProfileBases
description: Свойства списка и связей объектов windows10CertificateProfileBase.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27d9df3e386de8c19896d91e28a4d9b7819eec9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411899"
---
# <a name="list-windows10certificateprofilebases"></a><span data-ttu-id="f2928-103">Список windows10CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="f2928-103">List windows10CertificateProfileBases</span></span>

> <span data-ttu-id="f2928-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2928-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2928-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2928-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2928-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2928-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2928-107">Свойства списка и связей объектов [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="f2928-107">List properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2928-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f2928-108">Prerequisites</span></span>
<span data-ttu-id="f2928-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2928-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2928-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2928-111">Permission type</span></span>|<span data-ttu-id="f2928-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2928-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2928-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2928-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2928-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2928-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2928-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2928-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2928-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2928-116">Not supported.</span></span>|
|<span data-ttu-id="f2928-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2928-117">Application</span></span>|<span data-ttu-id="f2928-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2928-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2928-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2928-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2928-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2928-120">Request headers</span></span>
|<span data-ttu-id="f2928-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2928-121">Header</span></span>|<span data-ttu-id="f2928-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f2928-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2928-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2928-123">Authorization</span></span>|<span data-ttu-id="f2928-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f2928-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2928-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2928-125">Accept</span></span>|<span data-ttu-id="f2928-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2928-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2928-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2928-127">Request body</span></span>
<span data-ttu-id="f2928-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2928-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2928-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2928-129">Response</span></span>
<span data-ttu-id="f2928-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f2928-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2928-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f2928-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2928-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2928-132">Request</span></span>
<span data-ttu-id="f2928-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2928-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f2928-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2928-134">Response</span></span>
<span data-ttu-id="f2928-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f2928-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 811

{
  "value": [
    {
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
  ]
}
```




