---
title: Обновление deviceManagementExchangeOnPremisesPolicy
description: Обновление свойства объекта deviceManagementExchangeOnPremisesPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 633f1b80895bd84c27c57b5cee26aa286b1d0e49
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407209"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="0ede8-103">Обновление deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="0ede8-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="0ede8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ede8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ede8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ede8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ede8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ede8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ede8-107">Обновление свойства объекта [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0ede8-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ede8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0ede8-108">Prerequisites</span></span>
<span data-ttu-id="0ede8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ede8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ede8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ede8-111">Permission type</span></span>|<span data-ttu-id="0ede8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ede8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ede8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ede8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ede8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ede8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ede8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ede8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ede8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ede8-116">Not supported.</span></span>|
|<span data-ttu-id="0ede8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ede8-117">Application</span></span>|<span data-ttu-id="0ede8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ede8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ede8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ede8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0ede8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ede8-120">Request headers</span></span>
|<span data-ttu-id="0ede8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ede8-121">Header</span></span>|<span data-ttu-id="0ede8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ede8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ede8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ede8-123">Authorization</span></span>|<span data-ttu-id="0ede8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ede8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ede8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ede8-125">Accept</span></span>|<span data-ttu-id="0ede8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ede8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ede8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ede8-127">Request body</span></span>
<span data-ttu-id="0ede8-128">В тексте запроса укажите представление JSON для объекта [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0ede8-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="0ede8-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ede8-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="0ede8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ede8-130">Property</span></span>|<span data-ttu-id="0ede8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ede8-131">Type</span></span>|<span data-ttu-id="0ede8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ede8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ede8-133">id</span><span class="sxs-lookup"><span data-stu-id="0ede8-133">id</span></span>|<span data-ttu-id="0ede8-134">String</span><span class="sxs-lookup"><span data-stu-id="0ede8-134">String</span></span>|<span data-ttu-id="0ede8-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0ede8-135">Not yet documented</span></span>|
|<span data-ttu-id="0ede8-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="0ede8-136">notificationContent</span></span>|<span data-ttu-id="0ede8-137">Binary</span><span class="sxs-lookup"><span data-stu-id="0ede8-137">Binary</span></span>|<span data-ttu-id="0ede8-138">Текст уведомления, которое будет отправляться пользователям в карантин для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ede8-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="0ede8-139">Это массив байтов кодировке UTF8 HTML.</span><span class="sxs-lookup"><span data-stu-id="0ede8-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="0ede8-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0ede8-140">defaultAccessLevel</span></span>|[<span data-ttu-id="0ede8-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0ede8-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="0ede8-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ede8-142">Default access state in Exchange.</span></span> <span data-ttu-id="0ede8-143">Это правило применяется глобально во всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ede8-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="0ede8-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="0ede8-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="0ede8-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="0ede8-145">accessRules</span></span>|<span data-ttu-id="0ede8-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0ede8-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="0ede8-147">Список доступа устройств правила в Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ede8-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="0ede8-148">Правила доступа к применяются глобально во всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="0ede8-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="0ede8-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="0ede8-149">knownDeviceClasses</span></span>|<span data-ttu-id="0ede8-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0ede8-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="0ede8-151">Список классов устройств в Exchange</span><span class="sxs-lookup"><span data-stu-id="0ede8-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="0ede8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ede8-152">Response</span></span>
<span data-ttu-id="0ede8-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ede8-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ede8-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0ede8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ede8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ede8-155">Request</span></span>
<span data-ttu-id="0ede8-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ede8-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0ede8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ede8-157">Response</span></span>
<span data-ttu-id="0ede8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ede8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```




