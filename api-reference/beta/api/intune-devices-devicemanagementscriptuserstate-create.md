---
title: Создание deviceManagementScriptUserState
description: Создание нового объекта deviceManagementScriptUserState.
ms.openlocfilehash: 4d6aba6ae11f2d6250d20524a1e6f47e55bbda2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078686"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="6f256-103">Создание deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="6f256-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="6f256-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f256-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f256-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f256-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f256-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f256-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f256-107">Создание нового объекта [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6f256-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f256-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f256-108">Prerequisites</span></span>
<span data-ttu-id="6f256-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f256-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f256-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f256-111">Permission type</span></span>|<span data-ttu-id="6f256-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f256-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f256-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f256-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f256-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f256-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6f256-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f256-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f256-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f256-116">Not supported.</span></span>|
|<span data-ttu-id="6f256-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f256-117">Application</span></span>|<span data-ttu-id="6f256-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f256-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f256-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f256-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="6f256-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f256-120">Request headers</span></span>
|<span data-ttu-id="6f256-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f256-121">Header</span></span>|<span data-ttu-id="6f256-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f256-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f256-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f256-123">Authorization</span></span>|<span data-ttu-id="6f256-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f256-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f256-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f256-125">Accept</span></span>|<span data-ttu-id="6f256-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f256-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f256-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f256-127">Request body</span></span>
<span data-ttu-id="6f256-128">В тексте запроса укажите представление JSON для объекта deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="6f256-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="6f256-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="6f256-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="6f256-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f256-130">Property</span></span>|<span data-ttu-id="6f256-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f256-131">Type</span></span>|<span data-ttu-id="6f256-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f256-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f256-133">id</span><span class="sxs-lookup"><span data-stu-id="6f256-133">id</span></span>|<span data-ttu-id="6f256-134">String</span><span class="sxs-lookup"><span data-stu-id="6f256-134">String</span></span>|<span data-ttu-id="6f256-135">Ключ сущности состояние пользователя устройства управления скрипта.</span><span class="sxs-lookup"><span data-stu-id="6f256-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="6f256-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6f256-136">successDeviceCount</span></span>|<span data-ttu-id="6f256-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6f256-137">Int32</span></span>|<span data-ttu-id="6f256-138">Число допустимых устройства для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f256-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="6f256-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6f256-139">errorDeviceCount</span></span>|<span data-ttu-id="6f256-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6f256-140">Int32</span></span>|<span data-ttu-id="6f256-141">Число ошибок устройства для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f256-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="6f256-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f256-142">userPrincipalName</span></span>|<span data-ttu-id="6f256-143">String</span><span class="sxs-lookup"><span data-stu-id="6f256-143">String</span></span>|<span data-ttu-id="6f256-144">Имени участника-пользователя для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f256-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="6f256-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f256-145">Response</span></span>
<span data-ttu-id="6f256-146">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f256-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f256-147">Пример</span><span class="sxs-lookup"><span data-stu-id="6f256-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f256-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f256-148">Request</span></span>
<span data-ttu-id="6f256-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f256-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6f256-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f256-150">Response</span></span>
<span data-ttu-id="6f256-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6f256-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```





