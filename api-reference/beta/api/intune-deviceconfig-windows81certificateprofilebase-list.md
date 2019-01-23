---
title: Список windows81CertificateProfileBases
description: Свойства списка и связей объектов windows81CertificateProfileBase.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 906d3c968062de7350f464fc729208f63bc5f0ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417548"
---
# <a name="list-windows81certificateprofilebases"></a><span data-ttu-id="18809-103">Список windows81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="18809-103">List windows81CertificateProfileBases</span></span>

> <span data-ttu-id="18809-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18809-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18809-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18809-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18809-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18809-107">Свойства списка и связей объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="18809-107">List properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18809-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="18809-108">Prerequisites</span></span>
<span data-ttu-id="18809-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18809-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18809-111">Permission type</span></span>|<span data-ttu-id="18809-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18809-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18809-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18809-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18809-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18809-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18809-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18809-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18809-116">Not supported.</span></span>|
|<span data-ttu-id="18809-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18809-117">Application</span></span>|<span data-ttu-id="18809-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18809-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18809-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18809-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18809-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18809-120">Request headers</span></span>
|<span data-ttu-id="18809-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18809-121">Header</span></span>|<span data-ttu-id="18809-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18809-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18809-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18809-123">Authorization</span></span>|<span data-ttu-id="18809-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18809-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18809-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18809-125">Accept</span></span>|<span data-ttu-id="18809-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18809-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18809-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18809-127">Request body</span></span>
<span data-ttu-id="18809-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18809-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18809-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="18809-129">Response</span></span>
<span data-ttu-id="18809-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="18809-130">If successful, this method returns a `200 OK` response code and a collection of [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18809-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18809-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18809-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18809-132">Request</span></span>
<span data-ttu-id="18809-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18809-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18809-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="18809-134">Response</span></span>
<span data-ttu-id="18809-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18809-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
      "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```




