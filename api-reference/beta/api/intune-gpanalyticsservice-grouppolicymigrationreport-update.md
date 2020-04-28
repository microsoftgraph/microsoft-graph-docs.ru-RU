---
title: Обновление Граупполицимигратионрепорт
description: Обновление свойств объекта Граупполицимигратионрепорт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ab7e6b7a68dbc725f5fc4a875fd153a5f683df1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383759"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="44791-103">Обновление Граупполицимигратионрепорт</span><span class="sxs-lookup"><span data-stu-id="44791-103">Update groupPolicyMigrationReport</span></span>

<span data-ttu-id="44791-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44791-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44791-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44791-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44791-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44791-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44791-107">Обновление свойств объекта [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="44791-107">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44791-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44791-108">Prerequisites</span></span>
<span data-ttu-id="44791-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44791-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44791-111">Permission type</span></span>|<span data-ttu-id="44791-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44791-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44791-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44791-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44791-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44791-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44791-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44791-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44791-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44791-116">Not supported.</span></span>|
|<span data-ttu-id="44791-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44791-117">Application</span></span>|<span data-ttu-id="44791-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44791-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44791-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44791-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="44791-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44791-120">Request headers</span></span>
|<span data-ttu-id="44791-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44791-121">Header</span></span>|<span data-ttu-id="44791-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44791-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44791-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44791-123">Authorization</span></span>|<span data-ttu-id="44791-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44791-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44791-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44791-125">Accept</span></span>|<span data-ttu-id="44791-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44791-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44791-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44791-127">Request body</span></span>
<span data-ttu-id="44791-128">В тексте запроса добавьте представление объекта [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44791-128">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="44791-129">В следующей таблице приведены свойства, необходимые при создании [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span><span class="sxs-lookup"><span data-stu-id="44791-129">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="44791-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44791-130">Property</span></span>|<span data-ttu-id="44791-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44791-131">Type</span></span>|<span data-ttu-id="44791-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44791-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44791-133">id</span><span class="sxs-lookup"><span data-stu-id="44791-133">id</span></span>|<span data-ttu-id="44791-134">String</span><span class="sxs-lookup"><span data-stu-id="44791-134">String</span></span>|<span data-ttu-id="44791-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="44791-135">Not yet documented</span></span>|
|<span data-ttu-id="44791-136">граупполициобжектид</span><span class="sxs-lookup"><span data-stu-id="44791-136">groupPolicyObjectId</span></span>|<span data-ttu-id="44791-137">GUID</span><span class="sxs-lookup"><span data-stu-id="44791-137">Guid</span></span>|<span data-ttu-id="44791-138">GUID объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="44791-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="44791-139">displayName</span><span class="sxs-lookup"><span data-stu-id="44791-139">displayName</span></span>|<span data-ttu-id="44791-140">Строка</span><span class="sxs-lookup"><span data-stu-id="44791-140">String</span></span>|<span data-ttu-id="44791-141">Имя объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="44791-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="44791-142">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="44791-142">ouDistinguishedName</span></span>|<span data-ttu-id="44791-143">String</span><span class="sxs-lookup"><span data-stu-id="44791-143">String</span></span>|<span data-ttu-id="44791-144">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="44791-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="44791-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44791-145">createdDateTime</span></span>|<span data-ttu-id="44791-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44791-146">DateTimeOffset</span></span>|<span data-ttu-id="44791-147">Дата и время создания Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="44791-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="44791-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44791-148">lastModifiedDateTime</span></span>|<span data-ttu-id="44791-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44791-149">DateTimeOffset</span></span>|<span data-ttu-id="44791-150">Дата и время последнего изменения Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="44791-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="44791-151">граупполицикреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="44791-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="44791-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44791-152">DateTimeOffset</span></span>|<span data-ttu-id="44791-153">Дата и время создания Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="44791-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="44791-154">граупполициластмодифиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="44791-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="44791-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44791-155">DateTimeOffset</span></span>|<span data-ttu-id="44791-156">Дата и время последнего изменения Граупполицимигратионрепорт.</span><span class="sxs-lookup"><span data-stu-id="44791-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="44791-157">мигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="44791-157">migrationReadiness</span></span>|[<span data-ttu-id="44791-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="44791-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="44791-159">Область действия Intune для связанного файлового объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="44791-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="44791-160">Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="44791-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="44791-161">таржетединактиведиректори</span><span class="sxs-lookup"><span data-stu-id="44791-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="44791-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="44791-162">Boolean</span></span>|<span data-ttu-id="44791-163">Свойство Targeted в Active Directory из XML-контента объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="44791-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="44791-164">тоталсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="44791-164">totalSettingsCount</span></span>|<span data-ttu-id="44791-165">Int32</span><span class="sxs-lookup"><span data-stu-id="44791-165">Int32</span></span>|<span data-ttu-id="44791-166">Общее количество параметров групповой политики из файла GPO.</span><span class="sxs-lookup"><span data-stu-id="44791-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="44791-167">суппортедсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="44791-167">supportedSettingsCount</span></span>|<span data-ttu-id="44791-168">Int32</span><span class="sxs-lookup"><span data-stu-id="44791-168">Int32</span></span>|<span data-ttu-id="44791-169">Количество параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="44791-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="44791-170">суппортедсеттингсперцент</span><span class="sxs-lookup"><span data-stu-id="44791-170">supportedSettingsPercent</span></span>|<span data-ttu-id="44791-171">Int32</span><span class="sxs-lookup"><span data-stu-id="44791-171">Int32</span></span>|<span data-ttu-id="44791-172">Процент параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="44791-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="44791-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="44791-173">Response</span></span>
<span data-ttu-id="44791-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44791-174">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44791-175">Пример</span><span class="sxs-lookup"><span data-stu-id="44791-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="44791-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="44791-176">Request</span></span>
<span data-ttu-id="44791-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44791-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44791-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="44791-178">Response</span></span>
<span data-ttu-id="44791-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44791-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



