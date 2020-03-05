---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e03b6936d17297159115193a287bc96999c83d71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458933"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="02eda-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="02eda-103">Update deviceAppManagement</span></span>

<span data-ttu-id="02eda-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02eda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02eda-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02eda-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="02eda-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02eda-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02eda-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02eda-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02eda-108">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="02eda-108">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02eda-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02eda-109">Prerequisites</span></span>
<span data-ttu-id="02eda-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="02eda-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="02eda-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02eda-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="02eda-112">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="02eda-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="02eda-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02eda-113">Permission type</span></span>|<span data-ttu-id="02eda-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02eda-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="02eda-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02eda-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="02eda-116">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="02eda-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="02eda-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02eda-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="02eda-118">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="02eda-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="02eda-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02eda-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="02eda-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02eda-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02eda-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02eda-121">Not supported.</span></span> |
| <span data-ttu-id="02eda-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02eda-122">Application</span></span> | |
| <span data-ttu-id="02eda-123">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="02eda-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="02eda-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02eda-124">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="02eda-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="02eda-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="02eda-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02eda-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02eda-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02eda-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="02eda-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02eda-128">Request headers</span></span>
|<span data-ttu-id="02eda-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02eda-129">Header</span></span>|<span data-ttu-id="02eda-130">Значение</span><span class="sxs-lookup"><span data-stu-id="02eda-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02eda-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="02eda-131">Authorization</span></span>|<span data-ttu-id="02eda-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02eda-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02eda-133">Accept</span><span class="sxs-lookup"><span data-stu-id="02eda-133">Accept</span></span>|<span data-ttu-id="02eda-134">application/json</span><span class="sxs-lookup"><span data-stu-id="02eda-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02eda-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02eda-135">Request body</span></span>
<span data-ttu-id="02eda-136">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02eda-136">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="02eda-137">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="02eda-137">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="02eda-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="02eda-138">Property</span></span>|<span data-ttu-id="02eda-139">Тип</span><span class="sxs-lookup"><span data-stu-id="02eda-139">Type</span></span>|<span data-ttu-id="02eda-140">Описание</span><span class="sxs-lookup"><span data-stu-id="02eda-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02eda-141">id</span><span class="sxs-lookup"><span data-stu-id="02eda-141">id</span></span>|<span data-ttu-id="02eda-142">String</span><span class="sxs-lookup"><span data-stu-id="02eda-142">String</span></span>|<span data-ttu-id="02eda-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="02eda-143">Key of the entity.</span></span>|
|<span data-ttu-id="02eda-144">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="02eda-144">**On-boarding**</span></span>|
|<span data-ttu-id="02eda-145">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="02eda-145">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="02eda-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="02eda-146">Boolean</span></span>|<span data-ttu-id="02eda-147">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="02eda-147">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="02eda-148">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="02eda-148">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="02eda-149">String</span><span class="sxs-lookup"><span data-stu-id="02eda-149">String</span></span>|<span data-ttu-id="02eda-150">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="02eda-150">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="02eda-151">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="02eda-151">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="02eda-152">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="02eda-152">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="02eda-153">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="02eda-153">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="02eda-154">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="02eda-154">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="02eda-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="02eda-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="02eda-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02eda-156">DateTimeOffset</span></span>|<span data-ttu-id="02eda-157">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="02eda-157">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="02eda-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="02eda-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="02eda-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02eda-159">DateTimeOffset</span></span>|<span data-ttu-id="02eda-160">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="02eda-160">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="02eda-161">микрософтсторефорбусинесспорталселектион</span><span class="sxs-lookup"><span data-stu-id="02eda-161">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="02eda-162">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="02eda-162">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="02eda-163">Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune.</span><span class="sxs-lookup"><span data-stu-id="02eda-163">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="02eda-164">Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\]</span><span class="sxs-lookup"><span data-stu-id="02eda-164">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="02eda-165">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="02eda-165">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="02eda-166">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02eda-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="02eda-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="02eda-167">Response</span></span>
<span data-ttu-id="02eda-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02eda-168">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02eda-169">Пример</span><span class="sxs-lookup"><span data-stu-id="02eda-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="02eda-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="02eda-170">Request</span></span>

<span data-ttu-id="02eda-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02eda-171">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="02eda-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="02eda-172">Response</span></span>

<span data-ttu-id="02eda-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02eda-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```











