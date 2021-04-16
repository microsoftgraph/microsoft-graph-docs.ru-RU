---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc6e7cb6e7b5a5614f56048b586a47bbc2a0bcca
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864580"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="e0f7f-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="e0f7f-103">Update deviceAppManagement</span></span>

<span data-ttu-id="e0f7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0f7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0f7f-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0f7f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0f7f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0f7f-108">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e0f7f-108">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0f7f-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0f7f-109">Prerequisites</span></span>
<span data-ttu-id="e0f7f-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e0f7f-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0f7f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e0f7f-112">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="e0f7f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0f7f-113">Permission type</span></span>|<span data-ttu-id="e0f7f-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0f7f-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="e0f7f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0f7f-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="e0f7f-116">&nbsp;&nbsp; **Приложения,** **книги,** **onboarding,** **интеграция партнеров** или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="e0f7f-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="e0f7f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f7f-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e0f7f-118">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e0f7f-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e0f7f-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f7f-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e0f7f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0f7f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0f7f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-121">Not supported.</span></span> |
| <span data-ttu-id="e0f7f-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e0f7f-122">Application</span></span> | |
| <span data-ttu-id="e0f7f-123">&nbsp;&nbsp; **Приложения,** **книги,** **onboarding,** **интеграция партнеров** или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="e0f7f-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="e0f7f-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f7f-124">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e0f7f-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e0f7f-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e0f7f-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f7f-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0f7f-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0f7f-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="e0f7f-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0f7f-128">Request headers</span></span>
|<span data-ttu-id="e0f7f-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0f7f-129">Header</span></span>|<span data-ttu-id="e0f7f-130">Значение</span><span class="sxs-lookup"><span data-stu-id="e0f7f-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0f7f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0f7f-131">Authorization</span></span>|<span data-ttu-id="e0f7f-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0f7f-133">Accept</span><span class="sxs-lookup"><span data-stu-id="e0f7f-133">Accept</span></span>|<span data-ttu-id="e0f7f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e0f7f-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0f7f-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0f7f-135">Request body</span></span>
<span data-ttu-id="e0f7f-136">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-136">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="e0f7f-137">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e0f7f-137">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="e0f7f-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0f7f-138">Property</span></span>|<span data-ttu-id="e0f7f-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e0f7f-139">Type</span></span>|<span data-ttu-id="e0f7f-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f7f-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0f7f-141">id</span><span class="sxs-lookup"><span data-stu-id="e0f7f-141">id</span></span>|<span data-ttu-id="e0f7f-142">String</span><span class="sxs-lookup"><span data-stu-id="e0f7f-142">String</span></span>|<span data-ttu-id="e0f7f-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-143">Key of the entity.</span></span>|
|<span data-ttu-id="e0f7f-144">**На посадке**</span><span class="sxs-lookup"><span data-stu-id="e0f7f-144">**On-boarding**</span></span>|
|<span data-ttu-id="e0f7f-145">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="e0f7f-145">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="e0f7f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0f7f-146">Boolean</span></span>|<span data-ttu-id="e0f7f-147">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-147">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="e0f7f-148">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="e0f7f-148">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="e0f7f-149">String</span><span class="sxs-lookup"><span data-stu-id="e0f7f-149">String</span></span>|<span data-ttu-id="e0f7f-150">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-150">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="e0f7f-151">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-151">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="e0f7f-152">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e0f7f-152">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="e0f7f-153">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-153">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="e0f7f-154">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-154">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="e0f7f-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="e0f7f-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="e0f7f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0f7f-156">DateTimeOffset</span></span>|<span data-ttu-id="e0f7f-157">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-157">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="e0f7f-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e0f7f-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="e0f7f-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0f7f-159">DateTimeOffset</span></span>|<span data-ttu-id="e0f7f-160">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-160">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="e0f7f-161">MicrosoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="e0f7f-161">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="e0f7f-162">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="e0f7f-162">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="e0f7f-163">Сведения о портале конечных пользователей используются для синхронизации приложений из Microsoft Store для бизнеса на портал компании Intune.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-163">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="e0f7f-164">Существует три варианта выбора из "Только портала компании", "Портал компании и частный \[ магазин", "Только частный \] магазин".</span><span class="sxs-lookup"><span data-stu-id="e0f7f-164">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="e0f7f-165">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-165">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="e0f7f-166">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e0f7f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0f7f-167">Response</span></span>
<span data-ttu-id="e0f7f-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-168">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0f7f-169">Пример</span><span class="sxs-lookup"><span data-stu-id="e0f7f-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0f7f-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0f7f-170">Request</span></span>

<span data-ttu-id="e0f7f-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-171">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="e0f7f-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0f7f-172">Response</span></span>

<span data-ttu-id="e0f7f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0f7f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```










