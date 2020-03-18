---
title: Обновление Граупполицисеттингмаппинг
description: Обновление свойств объекта Граупполицисеттингмаппинг.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a98970a6bef6a17ab134322d1b9d41bfcd195ef5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804578"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="273c8-103">Обновление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="273c8-103">Update groupPolicySettingMapping</span></span>

> <span data-ttu-id="273c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="273c8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="273c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273c8-106">Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="273c8-106">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="273c8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="273c8-107">Prerequisites</span></span>
<span data-ttu-id="273c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="273c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="273c8-110">Permission type</span></span>|<span data-ttu-id="273c8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="273c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="273c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="273c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="273c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="273c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="273c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="273c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273c8-115">Not supported.</span></span>|
|<span data-ttu-id="273c8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="273c8-116">Application</span></span>|<span data-ttu-id="273c8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273c8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="273c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="273c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="273c8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="273c8-119">Request headers</span></span>
|<span data-ttu-id="273c8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="273c8-120">Header</span></span>|<span data-ttu-id="273c8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="273c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="273c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="273c8-122">Authorization</span></span>|<span data-ttu-id="273c8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="273c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="273c8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="273c8-124">Accept</span></span>|<span data-ttu-id="273c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="273c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="273c8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="273c8-126">Request body</span></span>
<span data-ttu-id="273c8-127">В тексте запроса добавьте представление объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="273c8-127">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="273c8-128">В следующей таблице приведены свойства, необходимые при создании [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="273c8-128">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="273c8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="273c8-129">Property</span></span>|<span data-ttu-id="273c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="273c8-130">Type</span></span>|<span data-ttu-id="273c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="273c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273c8-132">id</span><span class="sxs-lookup"><span data-stu-id="273c8-132">id</span></span>|<span data-ttu-id="273c8-133">String</span><span class="sxs-lookup"><span data-stu-id="273c8-133">String</span></span>|<span data-ttu-id="273c8-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c8-134">Not yet documented</span></span>|
|<span data-ttu-id="273c8-135">parentId</span><span class="sxs-lookup"><span data-stu-id="273c8-135">parentId</span></span>|<span data-ttu-id="273c8-136">String</span><span class="sxs-lookup"><span data-stu-id="273c8-136">String</span></span>|<span data-ttu-id="273c8-137">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="273c8-138">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="273c8-138">childIdList</span></span>|<span data-ttu-id="273c8-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="273c8-139">String collection</span></span>|<span data-ttu-id="273c8-140">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="273c8-141">settingName</span><span class="sxs-lookup"><span data-stu-id="273c8-141">settingName</span></span>|<span data-ttu-id="273c8-142">String</span><span class="sxs-lookup"><span data-stu-id="273c8-142">String</span></span>|<span data-ttu-id="273c8-143">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="273c8-144">settingValue</span></span>|<span data-ttu-id="273c8-145">String</span><span class="sxs-lookup"><span data-stu-id="273c8-145">String</span></span>|<span data-ttu-id="273c8-146">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-147">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="273c8-147">settingValueType</span></span>|<span data-ttu-id="273c8-148">String</span><span class="sxs-lookup"><span data-stu-id="273c8-148">String</span></span>|<span data-ttu-id="273c8-149">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-150">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="273c8-150">settingDisplayName</span></span>|<span data-ttu-id="273c8-151">String</span><span class="sxs-lookup"><span data-stu-id="273c8-151">String</span></span>|<span data-ttu-id="273c8-152">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-153">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="273c8-153">settingDisplayValue</span></span>|<span data-ttu-id="273c8-154">String</span><span class="sxs-lookup"><span data-stu-id="273c8-154">String</span></span>|<span data-ttu-id="273c8-155">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-156">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="273c8-156">settingDisplayValueType</span></span>|<span data-ttu-id="273c8-157">String</span><span class="sxs-lookup"><span data-stu-id="273c8-157">String</span></span>|<span data-ttu-id="273c8-158">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="273c8-159">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="273c8-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="273c8-160">String</span><span class="sxs-lookup"><span data-stu-id="273c8-160">String</span></span>|<span data-ttu-id="273c8-161">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="273c8-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="273c8-162">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="273c8-162">settingCategory</span></span>|<span data-ttu-id="273c8-163">String</span><span class="sxs-lookup"><span data-stu-id="273c8-163">String</span></span>|<span data-ttu-id="273c8-164">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="273c8-165">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="273c8-165">mdmCspName</span></span>|<span data-ttu-id="273c8-166">String</span><span class="sxs-lookup"><span data-stu-id="273c8-166">String</span></span>|<span data-ttu-id="273c8-167">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="273c8-168">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="273c8-168">mdmSettingUri</span></span>|<span data-ttu-id="273c8-169">String</span><span class="sxs-lookup"><span data-stu-id="273c8-169">String</span></span>|<span data-ttu-id="273c8-170">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="273c8-171">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="273c8-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="273c8-172">Int32</span><span class="sxs-lookup"><span data-stu-id="273c8-172">Int32</span></span>|<span data-ttu-id="273c8-173">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="273c8-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="273c8-174">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="273c8-174">settingType</span></span>|[<span data-ttu-id="273c8-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="273c8-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="273c8-176">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="273c8-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="273c8-177">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="273c8-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="273c8-178">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="273c8-178">isMdmSupported</span></span>|<span data-ttu-id="273c8-179">Логический</span><span class="sxs-lookup"><span data-stu-id="273c8-179">Boolean</span></span>|<span data-ttu-id="273c8-180">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="273c8-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="273c8-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="273c8-181">mdmSupportedState</span></span>|[<span data-ttu-id="273c8-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="273c8-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="273c8-183">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="273c8-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="273c8-184">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="273c8-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="273c8-185">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="273c8-185">settingScope</span></span>|[<span data-ttu-id="273c8-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="273c8-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="273c8-187">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="273c8-187">The scope of the setting.</span></span> <span data-ttu-id="273c8-188">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="273c8-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="273c8-189">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="273c8-189">intuneSettingUriList</span></span>|<span data-ttu-id="273c8-190">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="273c8-190">String collection</span></span>|<span data-ttu-id="273c8-191">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="273c8-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="273c8-192">интунесеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="273c8-192">intuneSettingDefinitionId</span></span>|<span data-ttu-id="273c8-193">String</span><span class="sxs-lookup"><span data-stu-id="273c8-193">String</span></span>|<span data-ttu-id="273c8-194">Идентификатор определения параметра Intune</span><span class="sxs-lookup"><span data-stu-id="273c8-194">The Intune Setting Definition Id</span></span>|



## <a name="response"></a><span data-ttu-id="273c8-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="273c8-195">Response</span></span>
<span data-ttu-id="273c8-196">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="273c8-196">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="273c8-197">Пример</span><span class="sxs-lookup"><span data-stu-id="273c8-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="273c8-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="273c8-198">Request</span></span>
<span data-ttu-id="273c8-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="273c8-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="273c8-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="273c8-200">Response</span></span>
<span data-ttu-id="273c8-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="273c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




