---
title: Получение Дефаултдевицекомплианцеполици
description: Чтение свойств и связей объекта Дефаултдевицекомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb95e01080b12823cf38158e1f63976ec9dc4a81
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084631"
---
# <a name="get-defaultdevicecompliancepolicy"></a><span data-ttu-id="5b380-103">Получение Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="5b380-103">Get defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="5b380-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b380-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b380-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b380-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b380-106">Чтение свойств и связей объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5b380-106">Read properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b380-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b380-107">Prerequisites</span></span>
<span data-ttu-id="5b380-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b380-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b380-110">Permission type</span></span>|<span data-ttu-id="5b380-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b380-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b380-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b380-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b380-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b380-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b380-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b380-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b380-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b380-115">Not supported.</span></span>|
|<span data-ttu-id="5b380-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b380-116">Application</span></span>|<span data-ttu-id="5b380-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b380-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b380-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b380-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b380-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b380-119">Optional query parameters</span></span>
<span data-ttu-id="5b380-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b380-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b380-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b380-121">Request headers</span></span>
|<span data-ttu-id="5b380-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b380-122">Header</span></span>|<span data-ttu-id="5b380-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5b380-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b380-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b380-124">Authorization</span></span>|<span data-ttu-id="5b380-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b380-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b380-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5b380-126">Accept</span></span>|<span data-ttu-id="5b380-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5b380-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b380-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b380-128">Request body</span></span>
<span data-ttu-id="5b380-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b380-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b380-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b380-130">Response</span></span>
<span data-ttu-id="5b380-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b380-131">If successful, this method returns a `200 OK` response code and [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b380-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5b380-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b380-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b380-133">Request</span></span>
<span data-ttu-id="5b380-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b380-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="5b380-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b380-135">Response</span></span>
<span data-ttu-id="5b380-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b380-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a285f027-f027-a285-27f0-85a227f085a2",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```






