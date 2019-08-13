---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89f77f0e39f8337136a428fb421143a65ff8ee35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351009"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="6fe1c-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6fe1c-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="6fe1c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fe1c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fe1c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe1c-107">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6fe1c-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fe1c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fe1c-108">Prerequisites</span></span>
<span data-ttu-id="6fe1c-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6fe1c-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe1c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6fe1c-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6fe1c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe1c-112">Permission type</span></span>|<span data-ttu-id="6fe1c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fe1c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="6fe1c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fe1c-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="6fe1c-115">&nbsp;&nbsp; **Приложения**, **книги**, входящая миграция или **Интеграция партнерских** **систем**</span><span class="sxs-lookup"><span data-stu-id="6fe1c-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, or **Partner Integration**</span></span> | <span data-ttu-id="6fe1c-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe1c-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6fe1c-117">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6fe1c-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6fe1c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe1c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6fe1c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fe1c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fe1c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-120">Not supported.</span></span> |
| <span data-ttu-id="6fe1c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fe1c-121">Application</span></span> | <span data-ttu-id="6fe1c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fe1c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fe1c-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="6fe1c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fe1c-124">Request headers</span></span>
|<span data-ttu-id="6fe1c-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fe1c-125">Header</span></span>|<span data-ttu-id="6fe1c-126">Значение</span><span class="sxs-lookup"><span data-stu-id="6fe1c-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe1c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fe1c-127">Authorization</span></span>|<span data-ttu-id="6fe1c-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe1c-129">Accept</span><span class="sxs-lookup"><span data-stu-id="6fe1c-129">Accept</span></span>|<span data-ttu-id="6fe1c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe1c-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe1c-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fe1c-131">Request body</span></span>
<span data-ttu-id="6fe1c-132">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="6fe1c-133">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6fe1c-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="6fe1c-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fe1c-134">Property</span></span>|<span data-ttu-id="6fe1c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="6fe1c-135">Type</span></span>|<span data-ttu-id="6fe1c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe1c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe1c-137">id</span><span class="sxs-lookup"><span data-stu-id="6fe1c-137">id</span></span>|<span data-ttu-id="6fe1c-138">String</span><span class="sxs-lookup"><span data-stu-id="6fe1c-138">String</span></span>|<span data-ttu-id="6fe1c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-139">Key of the entity.</span></span>|
|<span data-ttu-id="6fe1c-140">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="6fe1c-140">**On-boarding**</span></span>|
|<span data-ttu-id="6fe1c-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="6fe1c-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="6fe1c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fe1c-142">Boolean</span></span>|<span data-ttu-id="6fe1c-143">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="6fe1c-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="6fe1c-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="6fe1c-145">String</span><span class="sxs-lookup"><span data-stu-id="6fe1c-145">String</span></span>|<span data-ttu-id="6fe1c-146">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="6fe1c-147">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="6fe1c-148">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6fe1c-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="6fe1c-149">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="6fe1c-150">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="6fe1c-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="6fe1c-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="6fe1c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe1c-152">DateTimeOffset</span></span>|<span data-ttu-id="6fe1c-153">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="6fe1c-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe1c-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="6fe1c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe1c-155">DateTimeOffset</span></span>|<span data-ttu-id="6fe1c-156">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="6fe1c-157">микрософтсторефорбусинесспорталселектион</span><span class="sxs-lookup"><span data-stu-id="6fe1c-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="6fe1c-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="6fe1c-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="6fe1c-159">Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="6fe1c-160">Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\]</span><span class="sxs-lookup"><span data-stu-id="6fe1c-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="6fe1c-161">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="6fe1c-162">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="6fe1c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe1c-163">Response</span></span>
<span data-ttu-id="6fe1c-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe1c-165">Пример</span><span class="sxs-lookup"><span data-stu-id="6fe1c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe1c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fe1c-166">Request</span></span>

<span data-ttu-id="6fe1c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="6fe1c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe1c-168">Response</span></span>

<span data-ttu-id="6fe1c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fe1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```






