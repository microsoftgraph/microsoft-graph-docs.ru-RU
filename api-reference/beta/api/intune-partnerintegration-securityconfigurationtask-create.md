---
title: Создание Секуритиконфигуратионтаск
description: Создание нового объекта Секуритиконфигуратионтаск.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a145aed3721a869fb3cf716d6e3fa799a3efa3d2
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793494"
---
# <a name="create-securityconfigurationtask"></a><span data-ttu-id="08e1a-103">Создание Секуритиконфигуратионтаск</span><span class="sxs-lookup"><span data-stu-id="08e1a-103">Create securityConfigurationTask</span></span>

<span data-ttu-id="08e1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08e1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08e1a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08e1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08e1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e1a-107">Создание нового объекта [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) .</span><span class="sxs-lookup"><span data-stu-id="08e1a-107">Create a new [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08e1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08e1a-108">Prerequisites</span></span>
<span data-ttu-id="08e1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08e1a-111">Permission type</span></span>|<span data-ttu-id="08e1a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08e1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08e1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08e1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08e1a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e1a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08e1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08e1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08e1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e1a-116">Not supported.</span></span>|
|<span data-ttu-id="08e1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="08e1a-117">Application</span></span>|<span data-ttu-id="08e1a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e1a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08e1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08e1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="08e1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08e1a-120">Request headers</span></span>
|<span data-ttu-id="08e1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08e1a-121">Header</span></span>|<span data-ttu-id="08e1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08e1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08e1a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08e1a-123">Authorization</span></span>|<span data-ttu-id="08e1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08e1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08e1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08e1a-125">Accept</span></span>|<span data-ttu-id="08e1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08e1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08e1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08e1a-127">Request body</span></span>
<span data-ttu-id="08e1a-128">В тексте запроса добавьте представление объекта Секуритиконфигуратионтаск в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e1a-128">In the request body, supply a JSON representation for the securityConfigurationTask object.</span></span>

<span data-ttu-id="08e1a-129">В следующей таблице приведены свойства, необходимые при создании Секуритиконфигуратионтаск.</span><span class="sxs-lookup"><span data-stu-id="08e1a-129">The following table shows the properties that are required when you create the securityConfigurationTask.</span></span>

|<span data-ttu-id="08e1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08e1a-130">Property</span></span>|<span data-ttu-id="08e1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08e1a-131">Type</span></span>|<span data-ttu-id="08e1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08e1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e1a-133">id</span><span class="sxs-lookup"><span data-stu-id="08e1a-133">id</span></span>|<span data-ttu-id="08e1a-134">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-134">String</span></span>|<span data-ttu-id="08e1a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08e1a-135">The entity key.</span></span> <span data-ttu-id="08e1a-136">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="08e1a-137">displayName</span></span>|<span data-ttu-id="08e1a-138">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-138">String</span></span>|<span data-ttu-id="08e1a-139">Имя.</span><span class="sxs-lookup"><span data-stu-id="08e1a-139">The name.</span></span> <span data-ttu-id="08e1a-140">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-141">description</span><span class="sxs-lookup"><span data-stu-id="08e1a-141">description</span></span>|<span data-ttu-id="08e1a-142">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-142">String</span></span>|<span data-ttu-id="08e1a-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="08e1a-143">The description.</span></span> <span data-ttu-id="08e1a-144">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08e1a-145">createdDateTime</span></span>|<span data-ttu-id="08e1a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e1a-146">DateTimeOffset</span></span>|<span data-ttu-id="08e1a-147">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="08e1a-147">The created date.</span></span> <span data-ttu-id="08e1a-148">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="08e1a-149">dueDateTime</span></span>|<span data-ttu-id="08e1a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e1a-150">DateTimeOffset</span></span>|<span data-ttu-id="08e1a-151">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="08e1a-151">The due date.</span></span> <span data-ttu-id="08e1a-152">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-153">category</span><span class="sxs-lookup"><span data-stu-id="08e1a-153">category</span></span>|[<span data-ttu-id="08e1a-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="08e1a-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="08e1a-155">Категория.</span><span class="sxs-lookup"><span data-stu-id="08e1a-155">The category.</span></span> <span data-ttu-id="08e1a-156">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="08e1a-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="08e1a-157">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="08e1a-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="08e1a-158">priority</span><span class="sxs-lookup"><span data-stu-id="08e1a-158">priority</span></span>|[<span data-ttu-id="08e1a-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="08e1a-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="08e1a-160">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="08e1a-160">The priority.</span></span> <span data-ttu-id="08e1a-161">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="08e1a-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="08e1a-162">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="08e1a-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="08e1a-163">модуль</span><span class="sxs-lookup"><span data-stu-id="08e1a-163">creator</span></span>|<span data-ttu-id="08e1a-164">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-164">String</span></span>|<span data-ttu-id="08e1a-165">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="08e1a-165">The email address of the creator.</span></span> <span data-ttu-id="08e1a-166">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-167">креаторнотес</span><span class="sxs-lookup"><span data-stu-id="08e1a-167">creatorNotes</span></span>|<span data-ttu-id="08e1a-168">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-168">String</span></span>|<span data-ttu-id="08e1a-169">Заметки автора.</span><span class="sxs-lookup"><span data-stu-id="08e1a-169">Notes from the creator.</span></span> <span data-ttu-id="08e1a-170">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="08e1a-171">assignedTo</span></span>|<span data-ttu-id="08e1a-172">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-172">String</span></span>|<span data-ttu-id="08e1a-173">Имя или электронная почта администратора, которому назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="08e1a-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="08e1a-174">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="08e1a-175">status</span><span class="sxs-lookup"><span data-stu-id="08e1a-175">status</span></span>|[<span data-ttu-id="08e1a-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="08e1a-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="08e1a-177">Состояние.</span><span class="sxs-lookup"><span data-stu-id="08e1a-177">The status.</span></span> <span data-ttu-id="08e1a-178">Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="08e1a-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="08e1a-179">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="08e1a-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="08e1a-180">ендпоинтсекуритиполици</span><span class="sxs-lookup"><span data-stu-id="08e1a-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="08e1a-181">ендпоинтсекуритиконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="08e1a-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="08e1a-182">Тип политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="08e1a-182">The endpoint security policy type.</span></span> <span data-ttu-id="08e1a-183">Возможные значения: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span><span class="sxs-lookup"><span data-stu-id="08e1a-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="08e1a-184">аппликаблеплатформ</span><span class="sxs-lookup"><span data-stu-id="08e1a-184">applicablePlatform</span></span>|[<span data-ttu-id="08e1a-185">ендпоинтсекуритиконфигуратионаппликаблеплатформ</span><span class="sxs-lookup"><span data-stu-id="08e1a-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="08e1a-186">Соответствующая платформа.</span><span class="sxs-lookup"><span data-stu-id="08e1a-186">The applicable platform.</span></span> <span data-ttu-id="08e1a-187">Возможные значения: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span><span class="sxs-lookup"><span data-stu-id="08e1a-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="08e1a-188">ендпоинтсекуритиполиципрофиле</span><span class="sxs-lookup"><span data-stu-id="08e1a-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="08e1a-189">ендпоинтсекуритиконфигуратионпрофилетипе</span><span class="sxs-lookup"><span data-stu-id="08e1a-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="08e1a-190">Профиль политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="08e1a-190">The endpoint security policy profile.</span></span> <span data-ttu-id="08e1a-191">Возможные значения: `unknown` , `antivirus` ,,,,, `windowsSecurity` `bitLocker` `fileVault` `firewall` `firewallRules` ,,, `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` , `exploitProtection` , `webProtection` , `applicationControl` , `attackSurfaceReductionRules` , `accountProtection` .</span><span class="sxs-lookup"><span data-stu-id="08e1a-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="08e1a-192">insights</span><span class="sxs-lookup"><span data-stu-id="08e1a-192">insights</span></span>|<span data-ttu-id="08e1a-193">String</span><span class="sxs-lookup"><span data-stu-id="08e1a-193">String</span></span>|<span data-ttu-id="08e1a-194">Сведения об устранении.</span><span class="sxs-lookup"><span data-stu-id="08e1a-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="08e1a-195">манажеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="08e1a-195">managedDeviceCount</span></span>|<span data-ttu-id="08e1a-196">Int32</span><span class="sxs-lookup"><span data-stu-id="08e1a-196">Int32</span></span>|<span data-ttu-id="08e1a-197">Число уязвимых устройств.</span><span class="sxs-lookup"><span data-stu-id="08e1a-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="08e1a-198">интендедсеттингс</span><span class="sxs-lookup"><span data-stu-id="08e1a-198">intendedSettings</span></span>|<span data-ttu-id="08e1a-199">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="08e1a-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="08e1a-200">Предполагаемые параметры и их значения.</span><span class="sxs-lookup"><span data-stu-id="08e1a-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="08e1a-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="08e1a-201">Response</span></span>
<span data-ttu-id="08e1a-202">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08e1a-202">If successful, this method returns a `201 Created` response code and a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e1a-203">Пример</span><span class="sxs-lookup"><span data-stu-id="08e1a-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="08e1a-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="08e1a-204">Request</span></span>
<span data-ttu-id="08e1a-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08e1a-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="08e1a-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e1a-206">Response</span></span>
<span data-ttu-id="08e1a-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08e1a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



