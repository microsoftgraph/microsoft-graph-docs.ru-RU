---
title: Получение Секуритибаселинетемплате
description: Чтение свойств и связей объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a92c117aa894a6c8fc3da3977d2cff2d4f6fa525
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49282533"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="73471-103">Получение Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="73471-103">Get securityBaselineTemplate</span></span>

<span data-ttu-id="73471-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73471-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73471-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73471-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73471-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73471-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73471-107">Чтение свойств и связей объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="73471-107">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73471-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73471-108">Prerequisites</span></span>
<span data-ttu-id="73471-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73471-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73471-111">Permission type</span></span>|<span data-ttu-id="73471-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73471-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73471-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73471-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73471-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73471-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73471-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73471-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73471-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73471-116">Not supported.</span></span>|
|<span data-ttu-id="73471-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73471-117">Application</span></span>|<span data-ttu-id="73471-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73471-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73471-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73471-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73471-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73471-120">Optional query parameters</span></span>
<span data-ttu-id="73471-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73471-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73471-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73471-122">Request headers</span></span>
|<span data-ttu-id="73471-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73471-123">Header</span></span>|<span data-ttu-id="73471-124">Значение</span><span class="sxs-lookup"><span data-stu-id="73471-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73471-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73471-125">Authorization</span></span>|<span data-ttu-id="73471-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73471-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73471-127">Accept</span><span class="sxs-lookup"><span data-stu-id="73471-127">Accept</span></span>|<span data-ttu-id="73471-128">application/json</span><span class="sxs-lookup"><span data-stu-id="73471-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73471-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73471-129">Request body</span></span>
<span data-ttu-id="73471-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73471-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73471-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="73471-131">Response</span></span>
<span data-ttu-id="73471-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73471-132">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73471-133">Пример</span><span class="sxs-lookup"><span data-stu-id="73471-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="73471-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="73471-134">Request</span></span>
<span data-ttu-id="73471-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73471-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="73471-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="73471-136">Response</span></span>
<span data-ttu-id="73471-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73471-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineTemplate",
    "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
    "displayName": "Display Name value",
    "description": "Description value",
    "versionInfo": "Version Info value",
    "isDeprecated": true,
    "intentCount": 11,
    "templateType": "specializedDevices",
    "platformType": "androidForWork",
    "templateSubtype": "firewall",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```




