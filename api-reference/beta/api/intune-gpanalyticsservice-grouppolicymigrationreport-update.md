---
title: Обновление Граупполицимигратионрепорт
description: Обновление свойств объекта Граупполицимигратионрепорт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f22148ff9154abda2985d35a3f6aa92290cdca94
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804613"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="e52be-103">Обновление Граупполицимигратионрепорт</span><span class="sxs-lookup"><span data-stu-id="e52be-103">Update groupPolicyMigrationReport</span></span>

> <span data-ttu-id="e52be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e52be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e52be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e52be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e52be-106">Обновление свойств объекта [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="e52be-106">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e52be-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e52be-107">Prerequisites</span></span>
<span data-ttu-id="e52be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e52be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e52be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e52be-110">Permission type</span></span>|<span data-ttu-id="e52be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e52be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e52be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e52be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e52be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e52be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e52be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e52be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e52be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e52be-115">Not supported.</span></span>|
|<span data-ttu-id="e52be-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e52be-116">Application</span></span>|<span data-ttu-id="e52be-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e52be-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e52be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e52be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="e52be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e52be-119">Request headers</span></span>
|<span data-ttu-id="e52be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e52be-120">Header</span></span>|<span data-ttu-id="e52be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e52be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e52be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e52be-122">Authorization</span></span>|<span data-ttu-id="e52be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e52be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e52be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e52be-124">Accept</span></span>|<span data-ttu-id="e52be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e52be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e52be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e52be-126">Request body</span></span>
<span data-ttu-id="e52be-127">В тексте запроса добавьте представление объекта [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e52be-127">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="e52be-128">В следующей таблице приведены свойства, необходимые при создании [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span><span class="sxs-lookup"><span data-stu-id="e52be-128">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="e52be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e52be-129">Property</span></span>|<span data-ttu-id="e52be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e52be-130">Type</span></span>|<span data-ttu-id="e52be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e52be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e52be-132">id</span><span class="sxs-lookup"><span data-stu-id="e52be-132">id</span></span>|<span data-ttu-id="e52be-133">String</span><span class="sxs-lookup"><span data-stu-id="e52be-133">String</span></span>|<span data-ttu-id="e52be-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e52be-134">Not yet documented</span></span>|
|<span data-ttu-id="e52be-135">граупполициобжектид</span><span class="sxs-lookup"><span data-stu-id="e52be-135">groupPolicyObjectId</span></span>|<span data-ttu-id="e52be-136">GUID</span><span class="sxs-lookup"><span data-stu-id="e52be-136">Guid</span></span>|<span data-ttu-id="e52be-137">GUID объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="e52be-137">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="e52be-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e52be-138">displayName</span></span>|<span data-ttu-id="e52be-139">Строка</span><span class="sxs-lookup"><span data-stu-id="e52be-139">String</span></span>|<span data-ttu-id="e52be-140">Имя объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="e52be-140">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="e52be-141">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="e52be-141">ouDistinguishedName</span></span>|<span data-ttu-id="e52be-142">String</span><span class="sxs-lookup"><span data-stu-id="e52be-142">String</span></span>|<span data-ttu-id="e52be-143">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="e52be-143">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="e52be-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e52be-144">createdDateTime</span></span>|<span data-ttu-id="e52be-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52be-145">DateTimeOffset</span></span>|<span data-ttu-id="e52be-146">Дата и время создания Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="e52be-146">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="e52be-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e52be-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e52be-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52be-148">DateTimeOffset</span></span>|<span data-ttu-id="e52be-149">Дата и время последнего изменения Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="e52be-149">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="e52be-150">граупполицикреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="e52be-150">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="e52be-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52be-151">DateTimeOffset</span></span>|<span data-ttu-id="e52be-152">Дата и время создания Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="e52be-152">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="e52be-153">граупполициластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="e52be-153">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="e52be-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52be-154">DateTimeOffset</span></span>|<span data-ttu-id="e52be-155">Дата и время последнего изменения Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="e52be-155">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="e52be-156">мигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="e52be-156">migrationReadiness</span></span>|[<span data-ttu-id="e52be-157">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="e52be-157">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="e52be-158">Область действия Intune для связанного файлового объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e52be-158">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="e52be-159">Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e52be-159">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="e52be-160">таржетединактиведиректори</span><span class="sxs-lookup"><span data-stu-id="e52be-160">targetedInActiveDirectory</span></span>|<span data-ttu-id="e52be-161">Логический</span><span class="sxs-lookup"><span data-stu-id="e52be-161">Boolean</span></span>|<span data-ttu-id="e52be-162">Свойство Targeted в Active Directory из XML-контента объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="e52be-162">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="e52be-163">тоталсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="e52be-163">totalSettingsCount</span></span>|<span data-ttu-id="e52be-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e52be-164">Int32</span></span>|<span data-ttu-id="e52be-165">Общее количество параметров групповой политики из файла GPO.</span><span class="sxs-lookup"><span data-stu-id="e52be-165">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="e52be-166">суппортедсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="e52be-166">supportedSettingsCount</span></span>|<span data-ttu-id="e52be-167">Int32</span><span class="sxs-lookup"><span data-stu-id="e52be-167">Int32</span></span>|<span data-ttu-id="e52be-168">Количество параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="e52be-168">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="e52be-169">суппортедсеттингсперцент</span><span class="sxs-lookup"><span data-stu-id="e52be-169">supportedSettingsPercent</span></span>|<span data-ttu-id="e52be-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e52be-170">Int32</span></span>|<span data-ttu-id="e52be-171">Процент параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="e52be-171">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="e52be-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e52be-172">Response</span></span>
<span data-ttu-id="e52be-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e52be-173">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e52be-174">Пример</span><span class="sxs-lookup"><span data-stu-id="e52be-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="e52be-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="e52be-175">Request</span></span>
<span data-ttu-id="e52be-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e52be-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a><span data-ttu-id="e52be-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e52be-177">Response</span></span>
<span data-ttu-id="e52be-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e52be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```




