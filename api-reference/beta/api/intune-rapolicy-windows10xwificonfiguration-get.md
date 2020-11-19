---
title: Получение windows10XWifiConfiguration
description: Чтение свойств и связей объекта windows10XWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35d6a78754cee1908c1a530bea735ad9ce65c62f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242204"
---
# <a name="get-windows10xwificonfiguration"></a><span data-ttu-id="5f176-103">Получение windows10XWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f176-103">Get windows10XWifiConfiguration</span></span>

<span data-ttu-id="5f176-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f176-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f176-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f176-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f176-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f176-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f176-107">Чтение свойств и связей объекта [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5f176-107">Read properties and relationships of the [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f176-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f176-108">Prerequisites</span></span>
<span data-ttu-id="5f176-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f176-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f176-111">Permission type</span></span>|<span data-ttu-id="5f176-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f176-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f176-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f176-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f176-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f176-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5f176-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f176-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f176-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f176-116">Not supported.</span></span>|
|<span data-ttu-id="5f176-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5f176-117">Application</span></span>|<span data-ttu-id="5f176-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f176-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f176-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f176-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f176-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f176-120">Optional query parameters</span></span>
<span data-ttu-id="5f176-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5f176-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f176-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f176-122">Request headers</span></span>
|<span data-ttu-id="5f176-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f176-123">Header</span></span>|<span data-ttu-id="5f176-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5f176-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f176-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f176-125">Authorization</span></span>|<span data-ttu-id="5f176-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f176-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f176-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5f176-127">Accept</span></span>|<span data-ttu-id="5f176-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5f176-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f176-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f176-129">Request body</span></span>
<span data-ttu-id="5f176-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f176-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f176-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f176-131">Response</span></span>
<span data-ttu-id="5f176-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f176-132">If successful, this method returns a `200 OK` response code and [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f176-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5f176-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f176-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f176-134">Request</span></span>
<span data-ttu-id="5f176-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f176-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a><span data-ttu-id="5f176-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f176-136">Response</span></span>
<span data-ttu-id="5f176-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f176-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 605

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
    "id": "31063b86-3b86-3106-863b-0631863b0631",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
    "customXmlFileName": "Custom Xml File Name value",
    "customXml": "Y3VzdG9tWG1s"
  }
}
```




