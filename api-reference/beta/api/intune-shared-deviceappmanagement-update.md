---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5db3d2dc551c669a2244f5f86b452e5d1f83fd7e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537115"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="ea488-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="ea488-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="ea488-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea488-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea488-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea488-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea488-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea488-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea488-107">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ea488-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea488-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea488-108">Prerequisites</span></span>
<span data-ttu-id="ea488-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ea488-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ea488-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea488-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ea488-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="ea488-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="ea488-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea488-112">Permission type</span></span>|<span data-ttu-id="ea488-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea488-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="ea488-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea488-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="ea488-115">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="ea488-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="ea488-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea488-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ea488-117">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ea488-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ea488-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea488-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ea488-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea488-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea488-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea488-120">Not supported.</span></span> |
| <span data-ttu-id="ea488-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea488-121">Application</span></span> | |
| <span data-ttu-id="ea488-122">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="ea488-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="ea488-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea488-123">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ea488-124">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ea488-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ea488-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea488-125">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea488-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea488-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="ea488-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea488-127">Request headers</span></span>
|<span data-ttu-id="ea488-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea488-128">Header</span></span>|<span data-ttu-id="ea488-129">Значение</span><span class="sxs-lookup"><span data-stu-id="ea488-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea488-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea488-130">Authorization</span></span>|<span data-ttu-id="ea488-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea488-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea488-132">Accept</span><span class="sxs-lookup"><span data-stu-id="ea488-132">Accept</span></span>|<span data-ttu-id="ea488-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ea488-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea488-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea488-134">Request body</span></span>
<span data-ttu-id="ea488-135">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea488-135">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="ea488-136">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ea488-136">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="ea488-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea488-137">Property</span></span>|<span data-ttu-id="ea488-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ea488-138">Type</span></span>|<span data-ttu-id="ea488-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ea488-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea488-140">id</span><span class="sxs-lookup"><span data-stu-id="ea488-140">id</span></span>|<span data-ttu-id="ea488-141">String</span><span class="sxs-lookup"><span data-stu-id="ea488-141">String</span></span>|<span data-ttu-id="ea488-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea488-142">Key of the entity.</span></span>|
|<span data-ttu-id="ea488-143">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="ea488-143">**On-boarding**</span></span>|
|<span data-ttu-id="ea488-144">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="ea488-144">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="ea488-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea488-145">Boolean</span></span>|<span data-ttu-id="ea488-146">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ea488-146">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="ea488-147">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="ea488-147">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="ea488-148">String</span><span class="sxs-lookup"><span data-stu-id="ea488-148">String</span></span>|<span data-ttu-id="ea488-149">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ea488-149">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="ea488-150">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="ea488-150">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="ea488-151">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ea488-151">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="ea488-152">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="ea488-152">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="ea488-153">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="ea488-153">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="ea488-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="ea488-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="ea488-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea488-155">DateTimeOffset</span></span>|<span data-ttu-id="ea488-156">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ea488-156">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="ea488-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ea488-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ea488-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea488-158">DateTimeOffset</span></span>|<span data-ttu-id="ea488-159">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="ea488-159">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="ea488-160">микрософтсторефорбусинесспорталселектион</span><span class="sxs-lookup"><span data-stu-id="ea488-160">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="ea488-161">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="ea488-161">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="ea488-162">Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune.</span><span class="sxs-lookup"><span data-stu-id="ea488-162">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="ea488-163">Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\]</span><span class="sxs-lookup"><span data-stu-id="ea488-163">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="ea488-164">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="ea488-164">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="ea488-165">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea488-165">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="ea488-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea488-166">Response</span></span>
<span data-ttu-id="ea488-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea488-167">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea488-168">Пример</span><span class="sxs-lookup"><span data-stu-id="ea488-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea488-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea488-169">Request</span></span>

<span data-ttu-id="ea488-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea488-170">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="ea488-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea488-171">Response</span></span>

<span data-ttu-id="ea488-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea488-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









