---
title: Создание Граупполицисеттингмаппинг
description: Создание нового объекта Граупполицисеттингмаппинг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00b5a33b814d625d89f95be269638920f2ad16f0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270787"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="8c537-103">Создание Граупполицисеттингмаппинг</span><span class="sxs-lookup"><span data-stu-id="8c537-103">Create groupPolicySettingMapping</span></span>

<span data-ttu-id="8c537-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c537-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c537-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c537-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c537-107">Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="8c537-107">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c537-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c537-108">Prerequisites</span></span>
<span data-ttu-id="8c537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c537-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c537-111">Permission type</span></span>|<span data-ttu-id="8c537-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c537-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c537-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c537-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c537-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c537-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c537-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c537-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c537-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c537-116">Not supported.</span></span>|
|<span data-ttu-id="8c537-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c537-117">Application</span></span>|<span data-ttu-id="8c537-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c537-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c537-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c537-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="8c537-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c537-120">Request headers</span></span>
|<span data-ttu-id="8c537-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c537-121">Header</span></span>|<span data-ttu-id="8c537-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c537-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c537-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c537-123">Authorization</span></span>|<span data-ttu-id="8c537-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c537-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c537-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c537-125">Accept</span></span>|<span data-ttu-id="8c537-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c537-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c537-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c537-127">Request body</span></span>
<span data-ttu-id="8c537-128">В тексте запроса добавьте представление объекта Граупполицисеттингмаппинг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c537-128">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="8c537-129">В следующей таблице приведены свойства, необходимые при создании Граупполицисеттингмаппинг.</span><span class="sxs-lookup"><span data-stu-id="8c537-129">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="8c537-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c537-130">Property</span></span>|<span data-ttu-id="8c537-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c537-131">Type</span></span>|<span data-ttu-id="8c537-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c537-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c537-133">id</span><span class="sxs-lookup"><span data-stu-id="8c537-133">id</span></span>|<span data-ttu-id="8c537-134">String</span><span class="sxs-lookup"><span data-stu-id="8c537-134">String</span></span>|<span data-ttu-id="8c537-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c537-135">Not yet documented</span></span>|
|<span data-ttu-id="8c537-136">parentId</span><span class="sxs-lookup"><span data-stu-id="8c537-136">parentId</span></span>|<span data-ttu-id="8c537-137">String</span><span class="sxs-lookup"><span data-stu-id="8c537-137">String</span></span>|<span data-ttu-id="8c537-138">Родительский идентификатор параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="8c537-139">чилдидлист</span><span class="sxs-lookup"><span data-stu-id="8c537-139">childIdList</span></span>|<span data-ttu-id="8c537-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8c537-140">String collection</span></span>|<span data-ttu-id="8c537-141">Список дочерних идентификаторов параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="8c537-142">settingName</span><span class="sxs-lookup"><span data-stu-id="8c537-142">settingName</span></span>|<span data-ttu-id="8c537-143">String</span><span class="sxs-lookup"><span data-stu-id="8c537-143">String</span></span>|<span data-ttu-id="8c537-144">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="8c537-145">settingValue</span></span>|<span data-ttu-id="8c537-146">String</span><span class="sxs-lookup"><span data-stu-id="8c537-146">String</span></span>|<span data-ttu-id="8c537-147">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-148">сеттингвалуетипе</span><span class="sxs-lookup"><span data-stu-id="8c537-148">settingValueType</span></span>|<span data-ttu-id="8c537-149">String</span><span class="sxs-lookup"><span data-stu-id="8c537-149">String</span></span>|<span data-ttu-id="8c537-150">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-151">сеттингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="8c537-151">settingDisplayName</span></span>|<span data-ttu-id="8c537-152">String</span><span class="sxs-lookup"><span data-stu-id="8c537-152">String</span></span>|<span data-ttu-id="8c537-153">Отображаемое имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-154">сеттингдисплайвалуе</span><span class="sxs-lookup"><span data-stu-id="8c537-154">settingDisplayValue</span></span>|<span data-ttu-id="8c537-155">String</span><span class="sxs-lookup"><span data-stu-id="8c537-155">String</span></span>|<span data-ttu-id="8c537-156">Отображаемое значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-157">сеттингдисплайвалуетипе</span><span class="sxs-lookup"><span data-stu-id="8c537-157">settingDisplayValueType</span></span>|<span data-ttu-id="8c537-158">String</span><span class="sxs-lookup"><span data-stu-id="8c537-158">String</span></span>|<span data-ttu-id="8c537-159">Отображаемый тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="8c537-160">сеттингвалуедисплайунитс</span><span class="sxs-lookup"><span data-stu-id="8c537-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="8c537-161">String</span><span class="sxs-lookup"><span data-stu-id="8c537-161">String</span></span>|<span data-ttu-id="8c537-162">Отображаемые единицы значения параметра групповой политики</span><span class="sxs-lookup"><span data-stu-id="8c537-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="8c537-163">сеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="8c537-163">settingCategory</span></span>|<span data-ttu-id="8c537-164">String</span><span class="sxs-lookup"><span data-stu-id="8c537-164">String</span></span>|<span data-ttu-id="8c537-165">Категория, в которой находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="8c537-166">мдмкспнаме</span><span class="sxs-lookup"><span data-stu-id="8c537-166">mdmCspName</span></span>|<span data-ttu-id="8c537-167">String</span><span class="sxs-lookup"><span data-stu-id="8c537-167">String</span></span>|<span data-ttu-id="8c537-168">Имя CSP, которое сопоставляется параметру групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="8c537-169">мдмсеттингури</span><span class="sxs-lookup"><span data-stu-id="8c537-169">mdmSettingUri</span></span>|<span data-ttu-id="8c537-170">String</span><span class="sxs-lookup"><span data-stu-id="8c537-170">String</span></span>|<span data-ttu-id="8c537-171">Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="8c537-172">мдмминимумосверсион</span><span class="sxs-lookup"><span data-stu-id="8c537-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="8c537-173">Int32</span><span class="sxs-lookup"><span data-stu-id="8c537-173">Int32</span></span>|<span data-ttu-id="8c537-174">Минимальная версия ОС, поддерживаемая параметром MDM.</span><span class="sxs-lookup"><span data-stu-id="8c537-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="8c537-175">сеттингтипе</span><span class="sxs-lookup"><span data-stu-id="8c537-175">settingType</span></span>|[<span data-ttu-id="8c537-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="8c537-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="8c537-177">Тип параметра (Security или ADMX) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8c537-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="8c537-178">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="8c537-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="8c537-179">исмдмсуппортед</span><span class="sxs-lookup"><span data-stu-id="8c537-179">isMdmSupported</span></span>|<span data-ttu-id="8c537-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c537-180">Boolean</span></span>|<span data-ttu-id="8c537-181">Указывает, поддерживается ли Intune или нет</span><span class="sxs-lookup"><span data-stu-id="8c537-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="8c537-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="8c537-182">mdmSupportedState</span></span>|[<span data-ttu-id="8c537-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="8c537-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="8c537-184">Указывает, поддерживается ли параметр в MDM.</span><span class="sxs-lookup"><span data-stu-id="8c537-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="8c537-185">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="8c537-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="8c537-186">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="8c537-186">settingScope</span></span>|[<span data-ttu-id="8c537-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="8c537-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="8c537-188">Область применения параметра.</span><span class="sxs-lookup"><span data-stu-id="8c537-188">The scope of the setting.</span></span> <span data-ttu-id="8c537-189">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8c537-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="8c537-190">интунесеттингурилист</span><span class="sxs-lookup"><span data-stu-id="8c537-190">intuneSettingUriList</span></span>|<span data-ttu-id="8c537-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8c537-191">String collection</span></span>|<span data-ttu-id="8c537-192">Список URI параметров Intune, которые сопоставлены параметру групповой политики</span><span class="sxs-lookup"><span data-stu-id="8c537-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="8c537-193">интунесеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="8c537-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="8c537-194">String</span><span class="sxs-lookup"><span data-stu-id="8c537-194">String</span></span>|<span data-ttu-id="8c537-195">Идентификатор определения параметра Intune</span><span class="sxs-lookup"><span data-stu-id="8c537-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="8c537-196">адмкссеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="8c537-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="8c537-197">String</span><span class="sxs-lookup"><span data-stu-id="8c537-197">String</span></span>|<span data-ttu-id="8c537-198">Идентификатор групповой политики ADMX</span><span class="sxs-lookup"><span data-stu-id="8c537-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="8c537-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c537-199">Response</span></span>
<span data-ttu-id="8c537-200">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c537-200">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c537-201">Пример</span><span class="sxs-lookup"><span data-stu-id="8c537-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c537-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c537-202">Request</span></span>
<span data-ttu-id="8c537-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c537-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
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

### <a name="response"></a><span data-ttu-id="8c537-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c537-204">Response</span></span>
<span data-ttu-id="8c537-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c537-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




