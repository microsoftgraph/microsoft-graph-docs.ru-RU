---
title: Update groupPolicySettingMapping
description: Обновление свойств объекта groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82575a97badaba93f179c841502727e07ebff0af
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149830"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="8d80d-103">Update groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="8d80d-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="8d80d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d80d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d80d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d80d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d80d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d80d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d80d-107">Обновление свойств объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="8d80d-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d80d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d80d-108">Prerequisites</span></span>
<span data-ttu-id="8d80d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d80d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d80d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d80d-111">Permission type</span></span>|<span data-ttu-id="8d80d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d80d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d80d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d80d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d80d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d80d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d80d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d80d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d80d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d80d-116">Not supported.</span></span>|
|<span data-ttu-id="8d80d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d80d-117">Application</span></span>|<span data-ttu-id="8d80d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d80d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d80d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d80d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="8d80d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d80d-120">Request headers</span></span>
|<span data-ttu-id="8d80d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d80d-121">Header</span></span>|<span data-ttu-id="8d80d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d80d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d80d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d80d-123">Authorization</span></span>|<span data-ttu-id="8d80d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d80d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d80d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d80d-125">Accept</span></span>|<span data-ttu-id="8d80d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d80d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d80d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d80d-127">Request body</span></span>
<span data-ttu-id="8d80d-128">В теле запроса поставляем представление JSON для [объекта groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="8d80d-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="8d80d-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="8d80d-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="8d80d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d80d-130">Property</span></span>|<span data-ttu-id="8d80d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d80d-131">Type</span></span>|<span data-ttu-id="8d80d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d80d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d80d-133">id</span><span class="sxs-lookup"><span data-stu-id="8d80d-133">id</span></span>|<span data-ttu-id="8d80d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-134">String</span></span>|<span data-ttu-id="8d80d-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8d80d-135">Not yet documented</span></span>|
|<span data-ttu-id="8d80d-136">parentId</span><span class="sxs-lookup"><span data-stu-id="8d80d-136">parentId</span></span>|<span data-ttu-id="8d80d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-137">String</span></span>|<span data-ttu-id="8d80d-138">Родительский Id параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="8d80d-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="8d80d-139">childIdList</span></span>|<span data-ttu-id="8d80d-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8d80d-140">String collection</span></span>|<span data-ttu-id="8d80d-141">Список детских ид параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="8d80d-142">settingName</span><span class="sxs-lookup"><span data-stu-id="8d80d-142">settingName</span></span>|<span data-ttu-id="8d80d-143">String</span><span class="sxs-lookup"><span data-stu-id="8d80d-143">String</span></span>|<span data-ttu-id="8d80d-144">Имя этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="8d80d-145">settingValue</span></span>|<span data-ttu-id="8d80d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-146">String</span></span>|<span data-ttu-id="8d80d-147">Значение этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="8d80d-148">settingValueType</span></span>|<span data-ttu-id="8d80d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-149">String</span></span>|<span data-ttu-id="8d80d-150">Тип значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d80d-151">settingDisplayName</span></span>|<span data-ttu-id="8d80d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-152">String</span></span>|<span data-ttu-id="8d80d-153">Отображение имени этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="8d80d-154">settingDisplayValue</span></span>|<span data-ttu-id="8d80d-155">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-155">String</span></span>|<span data-ttu-id="8d80d-156">Отображение значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="8d80d-157">settingDisplayValueType</span></span>|<span data-ttu-id="8d80d-158">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-158">String</span></span>|<span data-ttu-id="8d80d-159">Тип отображения значения этого параметра групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="8d80d-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="8d80d-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="8d80d-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-161">String</span></span>|<span data-ttu-id="8d80d-162">Отображаемая единица этого значения групповой политики</span><span class="sxs-lookup"><span data-stu-id="8d80d-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="8d80d-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="8d80d-163">settingCategory</span></span>|<span data-ttu-id="8d80d-164">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-164">String</span></span>|<span data-ttu-id="8d80d-165">Категория, в которая находится параметр групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="8d80d-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="8d80d-166">mdmCspName</span></span>|<span data-ttu-id="8d80d-167">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-167">String</span></span>|<span data-ttu-id="8d80d-168">CSP назовет эту групповую политику, устанавливая карты.</span><span class="sxs-lookup"><span data-stu-id="8d80d-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="8d80d-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="8d80d-169">mdmSettingUri</span></span>|<span data-ttu-id="8d80d-170">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-170">String</span></span>|<span data-ttu-id="8d80d-171">MDM CSP URI этой групповой политики, устанавливая карты.</span><span class="sxs-lookup"><span data-stu-id="8d80d-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="8d80d-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="8d80d-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="8d80d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="8d80d-173">Int32</span></span>|<span data-ttu-id="8d80d-174">Минимальная версия ОС, поддерживаемая этим параметром mdm.</span><span class="sxs-lookup"><span data-stu-id="8d80d-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="8d80d-175">settingType</span><span class="sxs-lookup"><span data-stu-id="8d80d-175">settingType</span></span>|[<span data-ttu-id="8d80d-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="8d80d-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="8d80d-177">Тип параметра (безопасность или admx) групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8d80d-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="8d80d-178">Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span><span class="sxs-lookup"><span data-stu-id="8d80d-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="8d80d-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="8d80d-179">isMdmSupported</span></span>|<span data-ttu-id="8d80d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d80d-180">Boolean</span></span>|<span data-ttu-id="8d80d-181">Указывает, поддерживает ли параметр Intune или нет.</span><span class="sxs-lookup"><span data-stu-id="8d80d-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="8d80d-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="8d80d-182">mdmSupportedState</span></span>|[<span data-ttu-id="8d80d-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="8d80d-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="8d80d-184">Указывает, поддерживается ли параметр в Mdm или нет.</span><span class="sxs-lookup"><span data-stu-id="8d80d-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="8d80d-185">Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.</span><span class="sxs-lookup"><span data-stu-id="8d80d-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="8d80d-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="8d80d-186">settingScope</span></span>|[<span data-ttu-id="8d80d-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="8d80d-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="8d80d-188">Область настройки.</span><span class="sxs-lookup"><span data-stu-id="8d80d-188">The scope of the setting.</span></span> <span data-ttu-id="8d80d-189">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8d80d-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="8d80d-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="8d80d-190">intuneSettingUriList</span></span>|<span data-ttu-id="8d80d-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8d80d-191">String collection</span></span>|<span data-ttu-id="8d80d-192">Список URL-адресов intune Setting this group policy setting maps to</span><span class="sxs-lookup"><span data-stu-id="8d80d-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="8d80d-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8d80d-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="8d80d-194">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-194">String</span></span>|<span data-ttu-id="8d80d-195">Id определения параметра Intune</span><span class="sxs-lookup"><span data-stu-id="8d80d-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="8d80d-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8d80d-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="8d80d-197">Строка</span><span class="sxs-lookup"><span data-stu-id="8d80d-197">String</span></span>|<span data-ttu-id="8d80d-198">Admx Group Policy Id</span><span class="sxs-lookup"><span data-stu-id="8d80d-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="8d80d-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d80d-199">Response</span></span>
<span data-ttu-id="8d80d-200">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8d80d-200">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d80d-201">Пример</span><span class="sxs-lookup"><span data-stu-id="8d80d-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d80d-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d80d-202">Request</span></span>
<span data-ttu-id="8d80d-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d80d-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d80d-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d80d-204">Response</span></span>
<span data-ttu-id="8d80d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d80d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




