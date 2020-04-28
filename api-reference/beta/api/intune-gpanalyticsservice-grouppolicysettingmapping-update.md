---
title: Обновление Граупполицисеттингмаппинг
description: Обновление свойств объекта Граупполицисеттингмаппинг.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecc0098de9cc029c2c00874d1e1060e8827b747b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454830"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="dea48-103">Обновление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="dea48-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="dea48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dea48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dea48-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dea48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dea48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dea48-107">Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="dea48-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dea48-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dea48-108">Prerequisites</span></span>
<span data-ttu-id="dea48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dea48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dea48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dea48-111">Permission type</span></span>|<span data-ttu-id="dea48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dea48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dea48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dea48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dea48-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea48-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dea48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dea48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dea48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea48-116">Not supported.</span></span>|
|<span data-ttu-id="dea48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dea48-117">Application</span></span>|<span data-ttu-id="dea48-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea48-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dea48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dea48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="dea48-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dea48-120">Request headers</span></span>
|<span data-ttu-id="dea48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dea48-121">Header</span></span>|<span data-ttu-id="dea48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dea48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dea48-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dea48-123">Authorization</span></span>|<span data-ttu-id="dea48-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dea48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dea48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dea48-125">Accept</span></span>|<span data-ttu-id="dea48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dea48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dea48-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dea48-127">Request body</span></span>
<span data-ttu-id="dea48-128">В тексте запроса добавьте представление объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea48-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="dea48-129">В следующей таблице приведены свойства, необходимые при создании [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="dea48-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="dea48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea48-130">Property</span></span>|<span data-ttu-id="dea48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dea48-131">Type</span></span>|<span data-ttu-id="dea48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dea48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea48-133">id</span><span class="sxs-lookup"><span data-stu-id="dea48-133">id</span></span>|<span data-ttu-id="dea48-134">String</span><span class="sxs-lookup"><span data-stu-id="dea48-134">String</span></span>|<span data-ttu-id="dea48-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dea48-135">Not yet documented</span></span>|
|<span data-ttu-id="dea48-136">parentId</span><span class="sxs-lookup"><span data-stu-id="dea48-136">parentId</span></span>|<span data-ttu-id="dea48-137">String</span><span class="sxs-lookup"><span data-stu-id="dea48-137">String</span></span>|<span data-ttu-id="dea48-138">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="dea48-139">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="dea48-139">childIdList</span></span>|<span data-ttu-id="dea48-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="dea48-140">String collection</span></span>|<span data-ttu-id="dea48-141">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="dea48-142">settingName</span><span class="sxs-lookup"><span data-stu-id="dea48-142">settingName</span></span>|<span data-ttu-id="dea48-143">String</span><span class="sxs-lookup"><span data-stu-id="dea48-143">String</span></span>|<span data-ttu-id="dea48-144">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="dea48-145">settingValue</span></span>|<span data-ttu-id="dea48-146">String</span><span class="sxs-lookup"><span data-stu-id="dea48-146">String</span></span>|<span data-ttu-id="dea48-147">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-148">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="dea48-148">settingValueType</span></span>|<span data-ttu-id="dea48-149">String</span><span class="sxs-lookup"><span data-stu-id="dea48-149">String</span></span>|<span data-ttu-id="dea48-150">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-151">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="dea48-151">settingDisplayName</span></span>|<span data-ttu-id="dea48-152">String</span><span class="sxs-lookup"><span data-stu-id="dea48-152">String</span></span>|<span data-ttu-id="dea48-153">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-154">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="dea48-154">settingDisplayValue</span></span>|<span data-ttu-id="dea48-155">String</span><span class="sxs-lookup"><span data-stu-id="dea48-155">String</span></span>|<span data-ttu-id="dea48-156">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-157">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="dea48-157">settingDisplayValueType</span></span>|<span data-ttu-id="dea48-158">String</span><span class="sxs-lookup"><span data-stu-id="dea48-158">String</span></span>|<span data-ttu-id="dea48-159">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="dea48-160">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="dea48-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="dea48-161">String</span><span class="sxs-lookup"><span data-stu-id="dea48-161">String</span></span>|<span data-ttu-id="dea48-162">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="dea48-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="dea48-163">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="dea48-163">settingCategory</span></span>|<span data-ttu-id="dea48-164">String</span><span class="sxs-lookup"><span data-stu-id="dea48-164">String</span></span>|<span data-ttu-id="dea48-165">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="dea48-166">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="dea48-166">mdmCspName</span></span>|<span data-ttu-id="dea48-167">String</span><span class="sxs-lookup"><span data-stu-id="dea48-167">String</span></span>|<span data-ttu-id="dea48-168">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="dea48-169">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="dea48-169">mdmSettingUri</span></span>|<span data-ttu-id="dea48-170">String</span><span class="sxs-lookup"><span data-stu-id="dea48-170">String</span></span>|<span data-ttu-id="dea48-171">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="dea48-172">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="dea48-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="dea48-173">Int32</span><span class="sxs-lookup"><span data-stu-id="dea48-173">Int32</span></span>|<span data-ttu-id="dea48-174">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="dea48-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="dea48-175">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="dea48-175">settingType</span></span>|[<span data-ttu-id="dea48-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="dea48-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="dea48-177">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dea48-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="dea48-178">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="dea48-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="dea48-179">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="dea48-179">isMdmSupported</span></span>|<span data-ttu-id="dea48-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="dea48-180">Boolean</span></span>|<span data-ttu-id="dea48-181">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="dea48-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="dea48-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="dea48-182">mdmSupportedState</span></span>|[<span data-ttu-id="dea48-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="dea48-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="dea48-184">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="dea48-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="dea48-185">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="dea48-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="dea48-186">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="dea48-186">settingScope</span></span>|[<span data-ttu-id="dea48-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="dea48-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="dea48-188">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="dea48-188">The scope of the setting.</span></span> <span data-ttu-id="dea48-189">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="dea48-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="dea48-190">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="dea48-190">intuneSettingUriList</span></span>|<span data-ttu-id="dea48-191">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="dea48-191">String collection</span></span>|<span data-ttu-id="dea48-192">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="dea48-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="dea48-193">интунесеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="dea48-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="dea48-194">String</span><span class="sxs-lookup"><span data-stu-id="dea48-194">String</span></span>|<span data-ttu-id="dea48-195">Идентификатор определения параметра Intune</span><span class="sxs-lookup"><span data-stu-id="dea48-195">The Intune Setting Definition Id</span></span>|



## <a name="response"></a><span data-ttu-id="dea48-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="dea48-196">Response</span></span>
<span data-ttu-id="dea48-197">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dea48-197">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dea48-198">Пример</span><span class="sxs-lookup"><span data-stu-id="dea48-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="dea48-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="dea48-199">Request</span></span>
<span data-ttu-id="dea48-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dea48-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 957

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="dea48-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="dea48-201">Response</span></span>
<span data-ttu-id="dea48-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dea48-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1006

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```



