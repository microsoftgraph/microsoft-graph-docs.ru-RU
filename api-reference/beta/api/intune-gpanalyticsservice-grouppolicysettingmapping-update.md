---
title: Обновление Граупполицисеттингмаппинг
description: Обновление свойств объекта Граупполицисеттингмаппинг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 70bada190dd6f46ef3f8e0f87e31c847bf651d89
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043285"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="26e3a-103">Обновление Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="26e3a-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="26e3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26e3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26e3a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e3a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26e3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e3a-107">Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="26e3a-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26e3a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26e3a-108">Prerequisites</span></span>
<span data-ttu-id="26e3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e3a-111">Permission type</span></span>|<span data-ttu-id="26e3a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e3a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e3a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26e3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e3a-116">Not supported.</span></span>|
|<span data-ttu-id="26e3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e3a-117">Application</span></span>|<span data-ttu-id="26e3a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e3a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="26e3a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26e3a-120">Request headers</span></span>
|<span data-ttu-id="26e3a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26e3a-121">Header</span></span>|<span data-ttu-id="26e3a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26e3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e3a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e3a-123">Authorization</span></span>|<span data-ttu-id="26e3a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26e3a-125">Accept</span></span>|<span data-ttu-id="26e3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e3a-127">Request body</span></span>
<span data-ttu-id="26e3a-128">В тексте запроса добавьте представление объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e3a-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="26e3a-129">В следующей таблице приведены свойства, необходимые при создании [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span><span class="sxs-lookup"><span data-stu-id="26e3a-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="26e3a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e3a-130">Property</span></span>|<span data-ttu-id="26e3a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26e3a-131">Type</span></span>|<span data-ttu-id="26e3a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26e3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e3a-133">id</span><span class="sxs-lookup"><span data-stu-id="26e3a-133">id</span></span>|<span data-ttu-id="26e3a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-134">String</span></span>|<span data-ttu-id="26e3a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26e3a-135">Not yet documented</span></span>|
|<span data-ttu-id="26e3a-136">parentId</span><span class="sxs-lookup"><span data-stu-id="26e3a-136">parentId</span></span>|<span data-ttu-id="26e3a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-137">String</span></span>|<span data-ttu-id="26e3a-138">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="26e3a-139">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="26e3a-139">childIdList</span></span>|<span data-ttu-id="26e3a-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26e3a-140">String collection</span></span>|<span data-ttu-id="26e3a-141">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="26e3a-142">settingName</span><span class="sxs-lookup"><span data-stu-id="26e3a-142">settingName</span></span>|<span data-ttu-id="26e3a-143">String</span><span class="sxs-lookup"><span data-stu-id="26e3a-143">String</span></span>|<span data-ttu-id="26e3a-144">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="26e3a-145">settingValue</span></span>|<span data-ttu-id="26e3a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-146">String</span></span>|<span data-ttu-id="26e3a-147">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-148">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="26e3a-148">settingValueType</span></span>|<span data-ttu-id="26e3a-149">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-149">String</span></span>|<span data-ttu-id="26e3a-150">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-151">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="26e3a-151">settingDisplayName</span></span>|<span data-ttu-id="26e3a-152">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-152">String</span></span>|<span data-ttu-id="26e3a-153">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-154">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="26e3a-154">settingDisplayValue</span></span>|<span data-ttu-id="26e3a-155">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-155">String</span></span>|<span data-ttu-id="26e3a-156">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-157">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="26e3a-157">settingDisplayValueType</span></span>|<span data-ttu-id="26e3a-158">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-158">String</span></span>|<span data-ttu-id="26e3a-159">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="26e3a-160">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="26e3a-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="26e3a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-161">String</span></span>|<span data-ttu-id="26e3a-162">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="26e3a-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="26e3a-163">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="26e3a-163">settingCategory</span></span>|<span data-ttu-id="26e3a-164">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-164">String</span></span>|<span data-ttu-id="26e3a-165">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="26e3a-166">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="26e3a-166">mdmCspName</span></span>|<span data-ttu-id="26e3a-167">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-167">String</span></span>|<span data-ttu-id="26e3a-168">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="26e3a-169">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="26e3a-169">mdmSettingUri</span></span>|<span data-ttu-id="26e3a-170">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-170">String</span></span>|<span data-ttu-id="26e3a-171">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="26e3a-172">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="26e3a-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="26e3a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="26e3a-173">Int32</span></span>|<span data-ttu-id="26e3a-174">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="26e3a-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="26e3a-175">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="26e3a-175">settingType</span></span>|[<span data-ttu-id="26e3a-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="26e3a-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="26e3a-177">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="26e3a-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="26e3a-178">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="26e3a-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="26e3a-179">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="26e3a-179">isMdmSupported</span></span>|<span data-ttu-id="26e3a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="26e3a-180">Boolean</span></span>|<span data-ttu-id="26e3a-181">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="26e3a-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="26e3a-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="26e3a-182">mdmSupportedState</span></span>|[<span data-ttu-id="26e3a-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="26e3a-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="26e3a-184">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="26e3a-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="26e3a-185">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="26e3a-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="26e3a-186">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="26e3a-186">settingScope</span></span>|[<span data-ttu-id="26e3a-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="26e3a-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="26e3a-188">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="26e3a-188">The scope of the setting.</span></span> <span data-ttu-id="26e3a-189">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="26e3a-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="26e3a-190">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="26e3a-190">intuneSettingUriList</span></span>|<span data-ttu-id="26e3a-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26e3a-191">String collection</span></span>|<span data-ttu-id="26e3a-192">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="26e3a-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="26e3a-193">интунесеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="26e3a-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="26e3a-194">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-194">String</span></span>|<span data-ttu-id="26e3a-195">Идентификатор определения параметра Intune</span><span class="sxs-lookup"><span data-stu-id="26e3a-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="26e3a-196">адмкссеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="26e3a-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="26e3a-197">Строка</span><span class="sxs-lookup"><span data-stu-id="26e3a-197">String</span></span>|<span data-ttu-id="26e3a-198">Идентификатор групповой политики ADMX</span><span class="sxs-lookup"><span data-stu-id="26e3a-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="26e3a-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e3a-199">Response</span></span>
<span data-ttu-id="26e3a-200">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26e3a-200">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e3a-201">Пример</span><span class="sxs-lookup"><span data-stu-id="26e3a-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e3a-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e3a-202">Request</span></span>
<span data-ttu-id="26e3a-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e3a-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 1023

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="26e3a-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e3a-204">Response</span></span>
<span data-ttu-id="26e3a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e3a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1072

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```






