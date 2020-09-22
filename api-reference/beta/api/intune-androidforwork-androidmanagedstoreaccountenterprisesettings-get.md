---
title: Получение ресурса androidmanagedstoreaccountenterprisesettings
description: Чтение свойств и связей объекта ресурса androidmanagedstoreaccountenterprisesettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e975164fd8a2f5f7ab5f221ba719b7dba5c7864b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012602"
---
# <a name="get-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="01086-103">Получение ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="01086-103">Get androidManagedStoreAccountEnterpriseSettings</span></span>

<span data-ttu-id="01086-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01086-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01086-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01086-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01086-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01086-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01086-107">Чтение свойств и связей объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="01086-107">Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01086-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01086-108">Prerequisites</span></span>
<span data-ttu-id="01086-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01086-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01086-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01086-111">Permission type</span></span>|<span data-ttu-id="01086-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01086-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01086-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01086-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01086-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01086-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="01086-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01086-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01086-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01086-116">Not supported.</span></span>|
|<span data-ttu-id="01086-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01086-117">Application</span></span>|<span data-ttu-id="01086-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01086-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01086-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01086-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01086-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="01086-120">Optional query parameters</span></span>
<span data-ttu-id="01086-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01086-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01086-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01086-122">Request headers</span></span>
|<span data-ttu-id="01086-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01086-123">Header</span></span>|<span data-ttu-id="01086-124">Значение</span><span class="sxs-lookup"><span data-stu-id="01086-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01086-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="01086-125">Authorization</span></span>|<span data-ttu-id="01086-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01086-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01086-127">Accept</span><span class="sxs-lookup"><span data-stu-id="01086-127">Accept</span></span>|<span data-ttu-id="01086-128">application/json</span><span class="sxs-lookup"><span data-stu-id="01086-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01086-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01086-129">Request body</span></span>
<span data-ttu-id="01086-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01086-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01086-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01086-131">Response</span></span>
<span data-ttu-id="01086-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01086-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01086-133">Пример</span><span class="sxs-lookup"><span data-stu-id="01086-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="01086-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="01086-134">Request</span></span>
<span data-ttu-id="01086-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01086-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### <a name="response"></a><span data-ttu-id="01086-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="01086-136">Response</span></span>
<span data-ttu-id="01086-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01086-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1081

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
    "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true,
    "companyCodes": [
      {
        "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
        "enrollmentToken": "Enrollment Token value",
        "qrCodeContent": "Qr Code Content value",
        "qrCodeImage": {
          "@odata.type": "microsoft.graph.mimeContent",
          "type": "Type value",
          "value": "dmFsdWU="
        }
      }
    ],
    "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
  }
}
```






