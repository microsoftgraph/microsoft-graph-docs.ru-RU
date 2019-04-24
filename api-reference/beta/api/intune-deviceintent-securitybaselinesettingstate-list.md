---
title: Список Секуритибаселинесеттингстатес
description: Список свойств и связей объектов Секуритибаселинесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5954caa31cbb915df0713d412daf75e4291ebb6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466051"
---
# <a name="list-securitybaselinesettingstates"></a><span data-ttu-id="0b9ad-103">Список Секуритибаселинесеттингстатес</span><span class="sxs-lookup"><span data-stu-id="0b9ad-103">List securityBaselineSettingStates</span></span>

> <span data-ttu-id="0b9ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b9ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b9ad-106">Список свойств и связей объектов [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="0b9ad-106">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b9ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b9ad-107">Prerequisites</span></span>
<span data-ttu-id="0b9ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b9ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b9ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b9ad-110">Permission type</span></span>|<span data-ttu-id="0b9ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b9ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b9ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b9ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b9ad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b9ad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b9ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b9ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b9ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-115">Not supported.</span></span>|
|<span data-ttu-id="0b9ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b9ad-116">Application</span></span>|<span data-ttu-id="0b9ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b9ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b9ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

## <a name="request-headers"></a><span data-ttu-id="0b9ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b9ad-119">Request headers</span></span>
|<span data-ttu-id="0b9ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b9ad-120">Header</span></span>|<span data-ttu-id="0b9ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0b9ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b9ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b9ad-122">Authorization</span></span>|<span data-ttu-id="0b9ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b9ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b9ad-124">Accept</span></span>|<span data-ttu-id="0b9ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b9ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b9ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b9ad-126">Request body</span></span>
<span data-ttu-id="0b9ad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b9ad-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b9ad-128">Response</span></span>
<span data-ttu-id="0b9ad-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b9ad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0b9ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b9ad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b9ad-131">Request</span></span>
<span data-ttu-id="0b9ad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

### <a name="response"></a><span data-ttu-id="0b9ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b9ad-133">Response</span></span>
<span data-ttu-id="0b9ad-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineSettingState",
      "id": "798e520d-520d-798e-0d52-8e790d528e79",
      "settingName": "Setting Name value",
      "state": "secure",
      "settingCategoryId": "Setting Category Id value"
    }
  ]
}
```



