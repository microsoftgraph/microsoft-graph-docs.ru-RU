---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: tfitzmac
ms.openlocfilehash: 8e5dd8d24d69b20ad418d255f161646a6a252f50
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308367"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="1ca17-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="1ca17-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="1ca17-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ca17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ca17-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ca17-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ca17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ca17-107">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="1ca17-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ca17-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca17-108">Prerequisites</span></span>
<span data-ttu-id="1ca17-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca17-111">Permission type</span></span>|<span data-ttu-id="1ca17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ca17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ca17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca17-116">Not supported.</span></span>|
|<span data-ttu-id="1ca17-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca17-117">Application</span></span>|<span data-ttu-id="1ca17-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ca17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="1ca17-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ca17-120">Request headers</span></span>
|<span data-ttu-id="1ca17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ca17-121">Header</span></span>|<span data-ttu-id="1ca17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ca17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ca17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ca17-123">Authorization</span></span>|<span data-ttu-id="1ca17-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1ca17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ca17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ca17-125">Accept</span></span>|<span data-ttu-id="1ca17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ca17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ca17-127">Request body</span></span>
<span data-ttu-id="1ca17-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ca17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ca17-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ca17-129">Response</span></span>
<span data-ttu-id="1ca17-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1ca17-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ca17-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1ca17-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ca17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca17-132">Request</span></span>
<span data-ttu-id="1ca17-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ca17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="1ca17-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ca17-134">Response</span></span>
<span data-ttu-id="1ca17-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ca17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```





