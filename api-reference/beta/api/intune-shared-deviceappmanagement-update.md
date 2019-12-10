---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6abcaec953c07e6974d3a421ff26612710d390b2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940175"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="0856e-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="0856e-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="0856e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0856e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0856e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0856e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0856e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0856e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0856e-107">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0856e-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0856e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0856e-108">Prerequisites</span></span>
<span data-ttu-id="0856e-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="0856e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0856e-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0856e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="0856e-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="0856e-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="0856e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0856e-112">Permission type</span></span>|<span data-ttu-id="0856e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0856e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="0856e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0856e-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="0856e-115">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="0856e-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="0856e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0856e-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0856e-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0856e-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0856e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0856e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0856e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0856e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0856e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0856e-120">Not supported.</span></span> |
| <span data-ttu-id="0856e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0856e-121">Application</span></span> | |
| <span data-ttu-id="0856e-122">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="0856e-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="0856e-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0856e-123">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0856e-124">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0856e-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0856e-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0856e-125">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0856e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0856e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="0856e-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0856e-127">Request headers</span></span>
|<span data-ttu-id="0856e-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0856e-128">Header</span></span>|<span data-ttu-id="0856e-129">Значение</span><span class="sxs-lookup"><span data-stu-id="0856e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0856e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0856e-130">Authorization</span></span>|<span data-ttu-id="0856e-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0856e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0856e-132">Accept</span><span class="sxs-lookup"><span data-stu-id="0856e-132">Accept</span></span>|<span data-ttu-id="0856e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0856e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0856e-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0856e-134">Request body</span></span>
<span data-ttu-id="0856e-135">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0856e-135">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="0856e-136">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0856e-136">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="0856e-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="0856e-137">Property</span></span>|<span data-ttu-id="0856e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="0856e-138">Type</span></span>|<span data-ttu-id="0856e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="0856e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0856e-140">id</span><span class="sxs-lookup"><span data-stu-id="0856e-140">id</span></span>|<span data-ttu-id="0856e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0856e-141">String</span></span>|<span data-ttu-id="0856e-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0856e-142">Key of the entity.</span></span>|
|<span data-ttu-id="0856e-143">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="0856e-143">**On-boarding**</span></span>|
|<span data-ttu-id="0856e-144">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="0856e-144">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="0856e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0856e-145">Boolean</span></span>|<span data-ttu-id="0856e-146">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0856e-146">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="0856e-147">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="0856e-147">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="0856e-148">String</span><span class="sxs-lookup"><span data-stu-id="0856e-148">String</span></span>|<span data-ttu-id="0856e-149">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0856e-149">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="0856e-150">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="0856e-150">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="0856e-151">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="0856e-151">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="0856e-152">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="0856e-152">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="0856e-153">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="0856e-153">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="0856e-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="0856e-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="0856e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0856e-155">DateTimeOffset</span></span>|<span data-ttu-id="0856e-156">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0856e-156">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="0856e-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0856e-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0856e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0856e-158">DateTimeOffset</span></span>|<span data-ttu-id="0856e-159">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="0856e-159">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="0856e-160">микрософтсторефорбусинесспорталселектион</span><span class="sxs-lookup"><span data-stu-id="0856e-160">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="0856e-161">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="0856e-161">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="0856e-162">Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune.</span><span class="sxs-lookup"><span data-stu-id="0856e-162">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="0856e-163">Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\]</span><span class="sxs-lookup"><span data-stu-id="0856e-163">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="0856e-164">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="0856e-164">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="0856e-165">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0856e-165">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="0856e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0856e-166">Response</span></span>
<span data-ttu-id="0856e-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0856e-167">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0856e-168">Пример</span><span class="sxs-lookup"><span data-stu-id="0856e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0856e-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="0856e-169">Request</span></span>

<span data-ttu-id="0856e-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0856e-170">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="0856e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0856e-171">Response</span></span>

<span data-ttu-id="0856e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0856e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```











