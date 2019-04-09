---
title: Создание Секуритибаселинесеттингстате
description: Создание нового объекта Секуритибаселинесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01256dceacb34fb2b9e173ab671ab9f6b318449c
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523653"
---
# <a name="create-securitybaselinesettingstate"></a><span data-ttu-id="93745-103">Создание Секуритибаселинесеттингстате</span><span class="sxs-lookup"><span data-stu-id="93745-103">Create securityBaselineSettingState</span></span>

> <span data-ttu-id="93745-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93745-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93745-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93745-106">Создание нового объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="93745-106">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93745-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93745-107">Prerequisites</span></span>
<span data-ttu-id="93745-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93745-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93745-110">Permission type</span></span>|<span data-ttu-id="93745-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93745-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93745-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93745-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93745-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93745-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93745-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93745-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93745-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93745-115">Not supported.</span></span>|
|<span data-ttu-id="93745-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93745-116">Application</span></span>|<span data-ttu-id="93745-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93745-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93745-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93745-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

## <a name="request-headers"></a><span data-ttu-id="93745-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93745-119">Request headers</span></span>
|<span data-ttu-id="93745-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93745-120">Header</span></span>|<span data-ttu-id="93745-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93745-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93745-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93745-122">Authorization</span></span>|<span data-ttu-id="93745-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93745-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93745-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93745-124">Accept</span></span>|<span data-ttu-id="93745-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93745-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93745-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93745-126">Request body</span></span>
<span data-ttu-id="93745-127">В тексте запроса добавьте представление объекта Секуритибаселинесеттингстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93745-127">In the request body, supply a JSON representation for the securityBaselineSettingState object.</span></span>

<span data-ttu-id="93745-128">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинесеттингстате.</span><span class="sxs-lookup"><span data-stu-id="93745-128">The following table shows the properties that are required when you create the securityBaselineSettingState.</span></span>

|<span data-ttu-id="93745-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="93745-129">Property</span></span>|<span data-ttu-id="93745-130">Тип</span><span class="sxs-lookup"><span data-stu-id="93745-130">Type</span></span>|<span data-ttu-id="93745-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93745-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93745-132">id</span><span class="sxs-lookup"><span data-stu-id="93745-132">id</span></span>|<span data-ttu-id="93745-133">String</span><span class="sxs-lookup"><span data-stu-id="93745-133">String</span></span>|<span data-ttu-id="93745-134">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="93745-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="93745-135">settingName</span><span class="sxs-lookup"><span data-stu-id="93745-135">settingName</span></span>|<span data-ttu-id="93745-136">String</span><span class="sxs-lookup"><span data-stu-id="93745-136">String</span></span>|<span data-ttu-id="93745-137">Имя параметра, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="93745-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="93745-138">state</span><span class="sxs-lookup"><span data-stu-id="93745-138">state</span></span>|[<span data-ttu-id="93745-139">Секуритибаселинекомплианцестате</span><span class="sxs-lookup"><span data-stu-id="93745-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="93745-140">Состояние соответствия параметру базового уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="93745-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="93745-141">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="93745-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="93745-142">Сеттингкатегорид</span><span class="sxs-lookup"><span data-stu-id="93745-142">settingCategoryId</span></span>|<span data-ttu-id="93745-143">String</span><span class="sxs-lookup"><span data-stu-id="93745-143">String</span></span>|<span data-ttu-id="93745-144">Идентификатор категории параметров, к которой относится этот параметр</span><span class="sxs-lookup"><span data-stu-id="93745-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="93745-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="93745-145">Response</span></span>
<span data-ttu-id="93745-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93745-146">If successful, this method returns a `201 Created` response code and a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93745-147">Пример</span><span class="sxs-lookup"><span data-stu-id="93745-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="93745-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="93745-148">Request</span></span>
<span data-ttu-id="93745-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93745-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="93745-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="93745-150">Response</span></span>
<span data-ttu-id="93745-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93745-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```



