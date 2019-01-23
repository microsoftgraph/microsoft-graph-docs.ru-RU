---
title: Создание deviceManagementScriptUserState
description: Создание нового объекта deviceManagementScriptUserState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01ab54a736a5e9d1a305bff44a601494e8ec8860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424268"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="4fd64-103">Создание deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="4fd64-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="4fd64-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4fd64-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4fd64-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fd64-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fd64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fd64-107">Создание нового объекта [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="4fd64-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fd64-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4fd64-108">Prerequisites</span></span>
<span data-ttu-id="4fd64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fd64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fd64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fd64-111">Permission type</span></span>|<span data-ttu-id="4fd64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fd64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fd64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fd64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fd64-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fd64-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4fd64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fd64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fd64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd64-116">Not supported.</span></span>|
|<span data-ttu-id="4fd64-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fd64-117">Application</span></span>|<span data-ttu-id="4fd64-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fd64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fd64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="4fd64-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fd64-120">Request headers</span></span>
|<span data-ttu-id="4fd64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fd64-121">Header</span></span>|<span data-ttu-id="4fd64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fd64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fd64-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fd64-123">Authorization</span></span>|<span data-ttu-id="4fd64-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4fd64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fd64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fd64-125">Accept</span></span>|<span data-ttu-id="4fd64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fd64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fd64-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fd64-127">Request body</span></span>
<span data-ttu-id="4fd64-128">В тексте запроса укажите представление JSON для объекта deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="4fd64-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="4fd64-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="4fd64-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="4fd64-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fd64-130">Property</span></span>|<span data-ttu-id="4fd64-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd64-131">Type</span></span>|<span data-ttu-id="4fd64-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fd64-133">id</span><span class="sxs-lookup"><span data-stu-id="4fd64-133">id</span></span>|<span data-ttu-id="4fd64-134">String</span><span class="sxs-lookup"><span data-stu-id="4fd64-134">String</span></span>|<span data-ttu-id="4fd64-135">Ключ сущности состояние пользователя устройства управления скрипта.</span><span class="sxs-lookup"><span data-stu-id="4fd64-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="4fd64-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4fd64-136">successDeviceCount</span></span>|<span data-ttu-id="4fd64-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4fd64-137">Int32</span></span>|<span data-ttu-id="4fd64-138">Число допустимых устройства для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4fd64-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="4fd64-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4fd64-139">errorDeviceCount</span></span>|<span data-ttu-id="4fd64-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4fd64-140">Int32</span></span>|<span data-ttu-id="4fd64-141">Число ошибок устройства для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4fd64-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="4fd64-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fd64-142">userPrincipalName</span></span>|<span data-ttu-id="4fd64-143">String</span><span class="sxs-lookup"><span data-stu-id="4fd64-143">String</span></span>|<span data-ttu-id="4fd64-144">Имени участника-пользователя для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4fd64-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="4fd64-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fd64-145">Response</span></span>
<span data-ttu-id="4fd64-146">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4fd64-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fd64-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4fd64-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fd64-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fd64-148">Request</span></span>
<span data-ttu-id="4fd64-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fd64-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fd64-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fd64-150">Response</span></span>
<span data-ttu-id="4fd64-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4fd64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




