---
title: Создание groupPolicyMigrationReport
description: Создайте новый объект GroupPolicyMigrationReport.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08901e26346c1bae90e080e2bc2313c7cd46ed8d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135581"
---
# <a name="create-grouppolicymigrationreport"></a><span data-ttu-id="c25a4-103">Создание groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="c25a4-103">Create groupPolicyMigrationReport</span></span>

<span data-ttu-id="c25a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c25a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c25a4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c25a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c25a4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c25a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c25a4-107">Создайте новый [объект GroupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)</span><span class="sxs-lookup"><span data-stu-id="c25a4-107">Create a new [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c25a4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c25a4-108">Prerequisites</span></span>
<span data-ttu-id="c25a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c25a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c25a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c25a4-111">Permission type</span></span>|<span data-ttu-id="c25a4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c25a4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c25a4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c25a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c25a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c25a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c25a4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c25a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c25a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c25a4-116">Not supported.</span></span>|
|<span data-ttu-id="c25a4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c25a4-117">Application</span></span>|<span data-ttu-id="c25a4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c25a4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c25a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c25a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="c25a4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c25a4-120">Request headers</span></span>
|<span data-ttu-id="c25a4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c25a4-121">Header</span></span>|<span data-ttu-id="c25a4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c25a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c25a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c25a4-123">Authorization</span></span>|<span data-ttu-id="c25a4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c25a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c25a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c25a4-125">Accept</span></span>|<span data-ttu-id="c25a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c25a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c25a4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c25a4-127">Request body</span></span>
<span data-ttu-id="c25a4-128">В теле запроса поставляем представление JSON для объекта GroupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-128">In the request body, supply a JSON representation for the groupPolicyMigrationReport object.</span></span>

<span data-ttu-id="c25a4-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-129">The following table shows the properties that are required when you create the groupPolicyMigrationReport.</span></span>

|<span data-ttu-id="c25a4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c25a4-130">Property</span></span>|<span data-ttu-id="c25a4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c25a4-131">Type</span></span>|<span data-ttu-id="c25a4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c25a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c25a4-133">id</span><span class="sxs-lookup"><span data-stu-id="c25a4-133">id</span></span>|<span data-ttu-id="c25a4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c25a4-134">String</span></span>|<span data-ttu-id="c25a4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c25a4-135">Not yet documented</span></span>|
|<span data-ttu-id="c25a4-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="c25a4-136">groupPolicyObjectId</span></span>|<span data-ttu-id="c25a4-137">Guid</span><span class="sxs-lookup"><span data-stu-id="c25a4-137">Guid</span></span>|<span data-ttu-id="c25a4-138">GUID объекта групповой политики из контента GPO Xml</span><span class="sxs-lookup"><span data-stu-id="c25a4-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="c25a4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c25a4-139">displayName</span></span>|<span data-ttu-id="c25a4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c25a4-140">String</span></span>|<span data-ttu-id="c25a4-141">Имя объекта групповой политики из контента GPO Xml</span><span class="sxs-lookup"><span data-stu-id="c25a4-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="c25a4-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="c25a4-142">ouDistinguishedName</span></span>|<span data-ttu-id="c25a4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c25a4-143">String</span></span>|<span data-ttu-id="c25a4-144">Отличительное имя OU.</span><span class="sxs-lookup"><span data-stu-id="c25a4-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="c25a4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c25a4-145">createdDateTime</span></span>|<span data-ttu-id="c25a4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c25a4-146">DateTimeOffset</span></span>|<span data-ttu-id="c25a4-147">Дата и время создания GroupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="c25a4-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c25a4-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c25a4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c25a4-149">DateTimeOffset</span></span>|<span data-ttu-id="c25a4-150">Дата и время последнего изменения GroupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="c25a4-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c25a4-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="c25a4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c25a4-152">DateTimeOffset</span></span>|<span data-ttu-id="c25a4-153">Дата и время создания GroupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="c25a4-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c25a4-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="c25a4-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c25a4-155">DateTimeOffset</span></span>|<span data-ttu-id="c25a4-156">Дата и время последнего изменения GroupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="c25a4-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="c25a4-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="c25a4-157">migrationReadiness</span></span>|[<span data-ttu-id="c25a4-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="c25a4-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="c25a4-159">Покрытие Intune для связанного объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c25a4-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="c25a4-160">Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="c25a4-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="c25a4-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="c25a4-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="c25a4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c25a4-162">Boolean</span></span>|<span data-ttu-id="c25a4-163">Свойство Targeted in AD из GPO Xml Content</span><span class="sxs-lookup"><span data-stu-id="c25a4-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="c25a4-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="c25a4-164">totalSettingsCount</span></span>|<span data-ttu-id="c25a4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c25a4-165">Int32</span></span>|<span data-ttu-id="c25a4-166">Общее число параметров групповой политики из GPO-файла.</span><span class="sxs-lookup"><span data-stu-id="c25a4-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="c25a4-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="c25a4-167">supportedSettingsCount</span></span>|<span data-ttu-id="c25a4-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c25a4-168">Int32</span></span>|<span data-ttu-id="c25a4-169">Количество параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="c25a4-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="c25a4-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="c25a4-170">supportedSettingsPercent</span></span>|<span data-ttu-id="c25a4-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c25a4-171">Int32</span></span>|<span data-ttu-id="c25a4-172">Процент параметров групповой политики, поддерживаемых Intune.</span><span class="sxs-lookup"><span data-stu-id="c25a4-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="c25a4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25a4-173">Response</span></span>
<span data-ttu-id="c25a4-174">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c25a4-174">If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c25a4-175">Пример</span><span class="sxs-lookup"><span data-stu-id="c25a4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c25a4-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="c25a4-176">Request</span></span>
<span data-ttu-id="c25a4-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c25a4-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
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

### <a name="response"></a><span data-ttu-id="c25a4-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25a4-178">Response</span></span>
<span data-ttu-id="c25a4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c25a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




