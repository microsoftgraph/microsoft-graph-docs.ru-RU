---
title: Обновление securityConfigurationTask
description: Обновление свойств объекта securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d30ec94b815f06f17b790f8178544996ad98825
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134797"
---
# <a name="update-securityconfigurationtask"></a><span data-ttu-id="d23f7-103">Обновление securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="d23f7-103">Update securityConfigurationTask</span></span>

<span data-ttu-id="d23f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d23f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d23f7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d23f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d23f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d23f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d23f7-107">Обновление свойств объекта [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-107">Update the properties of a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d23f7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d23f7-108">Prerequisites</span></span>
<span data-ttu-id="d23f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d23f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d23f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d23f7-111">Permission type</span></span>|<span data-ttu-id="d23f7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d23f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d23f7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d23f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d23f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d23f7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d23f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d23f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d23f7-116">Not supported.</span></span>|
|<span data-ttu-id="d23f7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d23f7-117">Application</span></span>|<span data-ttu-id="d23f7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23f7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d23f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d23f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="d23f7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d23f7-120">Request headers</span></span>
|<span data-ttu-id="d23f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d23f7-121">Header</span></span>|<span data-ttu-id="d23f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d23f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d23f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d23f7-123">Authorization</span></span>|<span data-ttu-id="d23f7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d23f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d23f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d23f7-125">Accept</span></span>|<span data-ttu-id="d23f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d23f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d23f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d23f7-127">Request body</span></span>
<span data-ttu-id="d23f7-128">В теле запроса поставляем представление JSON для [объекта securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-128">In the request body, supply a JSON representation for the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

<span data-ttu-id="d23f7-129">В следующей таблице показаны свойства, необходимые при создании [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-129">The following table shows the properties that are required when you create the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).</span></span>

|<span data-ttu-id="d23f7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d23f7-130">Property</span></span>|<span data-ttu-id="d23f7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d23f7-131">Type</span></span>|<span data-ttu-id="d23f7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d23f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d23f7-133">id</span><span class="sxs-lookup"><span data-stu-id="d23f7-133">id</span></span>|<span data-ttu-id="d23f7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-134">String</span></span>|<span data-ttu-id="d23f7-135">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="d23f7-135">The entity key.</span></span> <span data-ttu-id="d23f7-136">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d23f7-137">displayName</span></span>|<span data-ttu-id="d23f7-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-138">String</span></span>|<span data-ttu-id="d23f7-139">Имя.</span><span class="sxs-lookup"><span data-stu-id="d23f7-139">The name.</span></span> <span data-ttu-id="d23f7-140">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-141">description</span><span class="sxs-lookup"><span data-stu-id="d23f7-141">description</span></span>|<span data-ttu-id="d23f7-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-142">String</span></span>|<span data-ttu-id="d23f7-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="d23f7-143">The description.</span></span> <span data-ttu-id="d23f7-144">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d23f7-145">createdDateTime</span></span>|<span data-ttu-id="d23f7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23f7-146">DateTimeOffset</span></span>|<span data-ttu-id="d23f7-147">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="d23f7-147">The created date.</span></span> <span data-ttu-id="d23f7-148">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d23f7-149">dueDateTime</span></span>|<span data-ttu-id="d23f7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23f7-150">DateTimeOffset</span></span>|<span data-ttu-id="d23f7-151">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="d23f7-151">The due date.</span></span> <span data-ttu-id="d23f7-152">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-153">category</span><span class="sxs-lookup"><span data-stu-id="d23f7-153">category</span></span>|[<span data-ttu-id="d23f7-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="d23f7-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="d23f7-155">Категория.</span><span class="sxs-lookup"><span data-stu-id="d23f7-155">The category.</span></span> <span data-ttu-id="d23f7-156">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d23f7-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d23f7-157">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="d23f7-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="d23f7-158">priority</span><span class="sxs-lookup"><span data-stu-id="d23f7-158">priority</span></span>|[<span data-ttu-id="d23f7-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="d23f7-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="d23f7-160">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="d23f7-160">The priority.</span></span> <span data-ttu-id="d23f7-161">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d23f7-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d23f7-162">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="d23f7-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="d23f7-163">creator</span><span class="sxs-lookup"><span data-stu-id="d23f7-163">creator</span></span>|<span data-ttu-id="d23f7-164">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-164">String</span></span>|<span data-ttu-id="d23f7-165">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="d23f7-165">The email address of the creator.</span></span> <span data-ttu-id="d23f7-166">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="d23f7-167">creatorNotes</span></span>|<span data-ttu-id="d23f7-168">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-168">String</span></span>|<span data-ttu-id="d23f7-169">Заметки от создателя.</span><span class="sxs-lookup"><span data-stu-id="d23f7-169">Notes from the creator.</span></span> <span data-ttu-id="d23f7-170">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d23f7-171">assignedTo</span></span>|<span data-ttu-id="d23f7-172">String</span><span class="sxs-lookup"><span data-stu-id="d23f7-172">String</span></span>|<span data-ttu-id="d23f7-173">Имя или электронная почта администратора этой задачи назначены.</span><span class="sxs-lookup"><span data-stu-id="d23f7-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="d23f7-174">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="d23f7-175">status</span><span class="sxs-lookup"><span data-stu-id="d23f7-175">status</span></span>|[<span data-ttu-id="d23f7-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="d23f7-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="d23f7-177">Состояние.</span><span class="sxs-lookup"><span data-stu-id="d23f7-177">The status.</span></span> <span data-ttu-id="d23f7-178">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="d23f7-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="d23f7-179">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="d23f7-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="d23f7-180">endpointSecurityPolicy</span><span class="sxs-lookup"><span data-stu-id="d23f7-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="d23f7-181">endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="d23f7-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="d23f7-182">Тип политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="d23f7-182">The endpoint security policy type.</span></span> <span data-ttu-id="d23f7-183">Возможные значения: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span><span class="sxs-lookup"><span data-stu-id="d23f7-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="d23f7-184">applicablePlatform</span><span class="sxs-lookup"><span data-stu-id="d23f7-184">applicablePlatform</span></span>|[<span data-ttu-id="d23f7-185">endpointSecurityConfigurationApplicablePlatform</span><span class="sxs-lookup"><span data-stu-id="d23f7-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="d23f7-186">Применимая платформа.</span><span class="sxs-lookup"><span data-stu-id="d23f7-186">The applicable platform.</span></span> <span data-ttu-id="d23f7-187">Возможные значения: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span><span class="sxs-lookup"><span data-stu-id="d23f7-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="d23f7-188">endpointSecurityPolicyProfile</span><span class="sxs-lookup"><span data-stu-id="d23f7-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="d23f7-189">endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="d23f7-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="d23f7-190">Профиль политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="d23f7-190">The endpoint security policy profile.</span></span> <span data-ttu-id="d23f7-191">Возможные значения: `unknown` `antivirus` , , , , , `windowsSecurity` , `bitLocker` , `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` , `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` , .</span><span class="sxs-lookup"><span data-stu-id="d23f7-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="d23f7-192">insights</span><span class="sxs-lookup"><span data-stu-id="d23f7-192">insights</span></span>|<span data-ttu-id="d23f7-193">Строка</span><span class="sxs-lookup"><span data-stu-id="d23f7-193">String</span></span>|<span data-ttu-id="d23f7-194">Сведения о смягчении последствий.</span><span class="sxs-lookup"><span data-stu-id="d23f7-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="d23f7-195">managedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d23f7-195">managedDeviceCount</span></span>|<span data-ttu-id="d23f7-196">Int32</span><span class="sxs-lookup"><span data-stu-id="d23f7-196">Int32</span></span>|<span data-ttu-id="d23f7-197">Количество уязвимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d23f7-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="d23f7-198">intendedSettings</span><span class="sxs-lookup"><span data-stu-id="d23f7-198">intendedSettings</span></span>|<span data-ttu-id="d23f7-199">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d23f7-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d23f7-200">Предполагаемые параметры и их значения.</span><span class="sxs-lookup"><span data-stu-id="d23f7-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="d23f7-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="d23f7-201">Response</span></span>
<span data-ttu-id="d23f7-202">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d23f7-202">If successful, this method returns a `200 OK` response code and an updated [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d23f7-203">Пример</span><span class="sxs-lookup"><span data-stu-id="d23f7-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="d23f7-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="d23f7-204">Request</span></span>
<span data-ttu-id="d23f7-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d23f7-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d23f7-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="d23f7-206">Response</span></span>
<span data-ttu-id="d23f7-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d23f7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "5d630f12-0f12-5d63-120f-635d120f635d",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




