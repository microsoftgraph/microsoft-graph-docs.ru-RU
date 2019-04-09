---
title: Обновление Секуритибаселинесеттингстате
description: Обновление свойств объекта Секуритибаселинесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3295cb35fbc9002f458a60d6f1b78a2ef380126b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524584"
---
# <a name="update-securitybaselinesettingstate"></a><span data-ttu-id="29693-103">Обновление Секуритибаселинесеттингстате</span><span class="sxs-lookup"><span data-stu-id="29693-103">Update securityBaselineSettingState</span></span>

> <span data-ttu-id="29693-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29693-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29693-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29693-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29693-106">Обновление свойств объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="29693-106">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29693-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="29693-107">Prerequisites</span></span>
<span data-ttu-id="29693-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="29693-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29693-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29693-110">Permission type</span></span>|<span data-ttu-id="29693-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29693-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29693-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29693-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29693-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29693-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29693-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29693-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29693-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29693-115">Not supported.</span></span>|
|<span data-ttu-id="29693-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29693-116">Application</span></span>|<span data-ttu-id="29693-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29693-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29693-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29693-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="29693-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29693-119">Request headers</span></span>
|<span data-ttu-id="29693-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29693-120">Header</span></span>|<span data-ttu-id="29693-121">Значение</span><span class="sxs-lookup"><span data-stu-id="29693-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29693-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29693-122">Authorization</span></span>|<span data-ttu-id="29693-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29693-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29693-124">Accept</span><span class="sxs-lookup"><span data-stu-id="29693-124">Accept</span></span>|<span data-ttu-id="29693-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29693-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29693-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29693-126">Request body</span></span>
<span data-ttu-id="29693-127">В тексте запроса добавьте представление объекта [Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29693-127">In the request body, supply a JSON representation for the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

<span data-ttu-id="29693-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="29693-128">The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

|<span data-ttu-id="29693-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="29693-129">Property</span></span>|<span data-ttu-id="29693-130">Тип</span><span class="sxs-lookup"><span data-stu-id="29693-130">Type</span></span>|<span data-ttu-id="29693-131">Описание</span><span class="sxs-lookup"><span data-stu-id="29693-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29693-132">id</span><span class="sxs-lookup"><span data-stu-id="29693-132">id</span></span>|<span data-ttu-id="29693-133">String</span><span class="sxs-lookup"><span data-stu-id="29693-133">String</span></span>|<span data-ttu-id="29693-134">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="29693-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="29693-135">settingName</span><span class="sxs-lookup"><span data-stu-id="29693-135">settingName</span></span>|<span data-ttu-id="29693-136">String</span><span class="sxs-lookup"><span data-stu-id="29693-136">String</span></span>|<span data-ttu-id="29693-137">Имя параметра, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="29693-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="29693-138">state</span><span class="sxs-lookup"><span data-stu-id="29693-138">state</span></span>|[<span data-ttu-id="29693-139">Секуритибаселинекомплианцестате</span><span class="sxs-lookup"><span data-stu-id="29693-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="29693-140">Состояние соответствия параметру базового уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="29693-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="29693-141">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="29693-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="29693-142">Сеттингкатегорид</span><span class="sxs-lookup"><span data-stu-id="29693-142">settingCategoryId</span></span>|<span data-ttu-id="29693-143">String</span><span class="sxs-lookup"><span data-stu-id="29693-143">String</span></span>|<span data-ttu-id="29693-144">Идентификатор категории параметров, к которой относится этот параметр</span><span class="sxs-lookup"><span data-stu-id="29693-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="29693-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="29693-145">Response</span></span>
<span data-ttu-id="29693-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29693-146">If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29693-147">Пример</span><span class="sxs-lookup"><span data-stu-id="29693-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="29693-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="29693-148">Request</span></span>
<span data-ttu-id="29693-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29693-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29693-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="29693-150">Response</span></span>
<span data-ttu-id="29693-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29693-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



