---
title: Обновление Мобилеаппинтентандстате
description: Обновление свойств объекта Мобилеаппинтентандстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d86e972fdef89297a23d719e3529ed73f0344b23
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350211"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="85429-103">Обновление Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="85429-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="85429-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85429-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85429-106">Обновление свойств объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="85429-106">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85429-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85429-107">Prerequisites</span></span>
<span data-ttu-id="85429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85429-110">Permission type</span></span>|<span data-ttu-id="85429-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85429-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="85429-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="85429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85429-115">Not supported.</span></span>|
|<span data-ttu-id="85429-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85429-116">Application</span></span>|<span data-ttu-id="85429-117">\* \* TODO: определение областей поддержка apponly \* \*</span><span class="sxs-lookup"><span data-stu-id="85429-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="85429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="85429-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85429-119">Request headers</span></span>
|<span data-ttu-id="85429-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85429-120">Header</span></span>|<span data-ttu-id="85429-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85429-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85429-122">Authorization</span></span>|<span data-ttu-id="85429-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85429-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85429-124">Accept</span></span>|<span data-ttu-id="85429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85429-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85429-126">Request body</span></span>
<span data-ttu-id="85429-127">В тексте запроса добавьте представление объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85429-127">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="85429-128">В следующей таблице приведены свойства, необходимые при создании [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="85429-128">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="85429-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85429-129">Property</span></span>|<span data-ttu-id="85429-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85429-130">Type</span></span>|<span data-ttu-id="85429-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85429-132">id</span><span class="sxs-lookup"><span data-stu-id="85429-132">id</span></span>|<span data-ttu-id="85429-133">Строка</span><span class="sxs-lookup"><span data-stu-id="85429-133">String</span></span>|<span data-ttu-id="85429-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="85429-134">UUID for the object</span></span>|
|<span data-ttu-id="85429-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="85429-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="85429-136">String</span><span class="sxs-lookup"><span data-stu-id="85429-136">String</span></span>|<span data-ttu-id="85429-137">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="85429-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="85429-138">userId</span><span class="sxs-lookup"><span data-stu-id="85429-138">userId</span></span>|<span data-ttu-id="85429-139">String</span><span class="sxs-lookup"><span data-stu-id="85429-139">String</span></span>|<span data-ttu-id="85429-140">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="85429-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="85429-141">мобилеапплист</span><span class="sxs-lookup"><span data-stu-id="85429-141">mobileAppList</span></span>|<span data-ttu-id="85429-142">Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="85429-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="85429-143">Список целей и состояний полезных данных для клиента.</span><span class="sxs-lookup"><span data-stu-id="85429-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="85429-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="85429-144">Response</span></span>
<span data-ttu-id="85429-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85429-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85429-146">Пример</span><span class="sxs-lookup"><span data-stu-id="85429-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="85429-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="85429-147">Request</span></span>
<span data-ttu-id="85429-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85429-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="85429-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="85429-149">Response</span></span>
<span data-ttu-id="85429-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```






