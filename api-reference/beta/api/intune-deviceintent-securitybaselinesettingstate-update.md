---
title: Обновление Секуритибаселинесеттингстате
description: Обновление свойств объекта Секуритибаселинесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c65f3c49159f6025ae32ee9a12c7acc395742509
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466128"
---
# <a name="update-securitybaselinesettingstate"></a><span data-ttu-id="ec8b5-103">Обновление Секуритибаселинесеттингстате</span><span class="sxs-lookup"><span data-stu-id="ec8b5-103">Update securityBaselineSettingState</span></span>

> <span data-ttu-id="ec8b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec8b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec8b5-106">Обновление свойств объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ec8b5-106">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec8b5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec8b5-107">Prerequisites</span></span>
<span data-ttu-id="ec8b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec8b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec8b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec8b5-110">Permission type</span></span>|<span data-ttu-id="ec8b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec8b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec8b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec8b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec8b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec8b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec8b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec8b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec8b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-115">Not supported.</span></span>|
|<span data-ttu-id="ec8b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec8b5-116">Application</span></span>|<span data-ttu-id="ec8b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec8b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec8b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ec8b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec8b5-119">Request headers</span></span>
|<span data-ttu-id="ec8b5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec8b5-120">Header</span></span>|<span data-ttu-id="ec8b5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec8b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec8b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec8b5-122">Authorization</span></span>|<span data-ttu-id="ec8b5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec8b5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ec8b5-124">Accept</span></span>|<span data-ttu-id="ec8b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec8b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec8b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec8b5-126">Request body</span></span>
<span data-ttu-id="ec8b5-127">В тексте запроса добавьте представление объекта [Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-127">In the request body, supply a JSON representation for the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

<span data-ttu-id="ec8b5-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="ec8b5-128">The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

|<span data-ttu-id="ec8b5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec8b5-129">Property</span></span>|<span data-ttu-id="ec8b5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ec8b5-130">Type</span></span>|<span data-ttu-id="ec8b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ec8b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8b5-132">id</span><span class="sxs-lookup"><span data-stu-id="ec8b5-132">id</span></span>|<span data-ttu-id="ec8b5-133">String</span><span class="sxs-lookup"><span data-stu-id="ec8b5-133">String</span></span>|<span data-ttu-id="ec8b5-134">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="ec8b5-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="ec8b5-135">settingName</span><span class="sxs-lookup"><span data-stu-id="ec8b5-135">settingName</span></span>|<span data-ttu-id="ec8b5-136">String</span><span class="sxs-lookup"><span data-stu-id="ec8b5-136">String</span></span>|<span data-ttu-id="ec8b5-137">Имя параметра, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="ec8b5-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="ec8b5-138">state</span><span class="sxs-lookup"><span data-stu-id="ec8b5-138">state</span></span>|[<span data-ttu-id="ec8b5-139">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="ec8b5-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="ec8b5-140">Состояние соответствия параметру базового уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="ec8b5-141">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="ec8b5-142">Сеттингкатегорид</span><span class="sxs-lookup"><span data-stu-id="ec8b5-142">settingCategoryId</span></span>|<span data-ttu-id="ec8b5-143">String</span><span class="sxs-lookup"><span data-stu-id="ec8b5-143">String</span></span>|<span data-ttu-id="ec8b5-144">Идентификатор категории параметров, к которой относится этот параметр</span><span class="sxs-lookup"><span data-stu-id="ec8b5-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="ec8b5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec8b5-145">Response</span></span>
<span data-ttu-id="ec8b5-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-146">If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec8b5-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ec8b5-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec8b5-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec8b5-148">Request</span></span>
<span data-ttu-id="ec8b5-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="ec8b5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec8b5-150">Response</span></span>
<span data-ttu-id="ec8b5-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec8b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



