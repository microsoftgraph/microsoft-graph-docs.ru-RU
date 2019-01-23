---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6067640d883e771d79e925fd0bcf87c2857c2c0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412809"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="b6a43-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b6a43-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="b6a43-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6a43-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6a43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6a43-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6a43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6a43-107">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b6a43-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6a43-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b6a43-108">Prerequisites</span></span>
<span data-ttu-id="b6a43-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b6a43-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6a43-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a43-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b6a43-111">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="b6a43-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b6a43-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a43-112">Permission type</span></span>|<span data-ttu-id="b6a43-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6a43-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="b6a43-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a43-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b6a43-115">&nbsp;&nbsp; **Приложений**, **книги**или **адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="b6a43-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="b6a43-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a43-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b6a43-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b6a43-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b6a43-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a43-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b6a43-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a43-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a43-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a43-120">Not supported.</span></span> |
| <span data-ttu-id="b6a43-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a43-121">Application</span></span> | <span data-ttu-id="b6a43-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a43-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a43-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a43-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="b6a43-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a43-124">Request headers</span></span>
|<span data-ttu-id="b6a43-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6a43-125">Header</span></span>|<span data-ttu-id="b6a43-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b6a43-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6a43-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6a43-127">Authorization</span></span>|<span data-ttu-id="b6a43-128">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6a43-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6a43-129">Accept</span><span class="sxs-lookup"><span data-stu-id="b6a43-129">Accept</span></span>|<span data-ttu-id="b6a43-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a43-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a43-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6a43-131">Request body</span></span>
<span data-ttu-id="b6a43-132">В теле запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6a43-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="b6a43-133">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b6a43-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="b6a43-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6a43-134">Property</span></span>|<span data-ttu-id="b6a43-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a43-135">Type</span></span>|<span data-ttu-id="b6a43-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a43-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a43-137">id</span><span class="sxs-lookup"><span data-stu-id="b6a43-137">id</span></span>|<span data-ttu-id="b6a43-138">String</span><span class="sxs-lookup"><span data-stu-id="b6a43-138">String</span></span>|<span data-ttu-id="b6a43-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6a43-139">Key of the entity.</span></span>|
|<span data-ttu-id="b6a43-140">**На использование доски**</span><span class="sxs-lookup"><span data-stu-id="b6a43-140">**On-boarding**</span></span>|
|<span data-ttu-id="b6a43-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="b6a43-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="b6a43-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6a43-142">Boolean</span></span>|<span data-ttu-id="b6a43-143">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b6a43-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="b6a43-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="b6a43-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="b6a43-145">String</span><span class="sxs-lookup"><span data-stu-id="b6a43-145">String</span></span>|<span data-ttu-id="b6a43-146">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b6a43-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="b6a43-147">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="b6a43-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="b6a43-148">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b6a43-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="b6a43-149">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="b6a43-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="b6a43-150">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="b6a43-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="b6a43-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="b6a43-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="b6a43-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6a43-152">DateTimeOffset</span></span>|<span data-ttu-id="b6a43-153">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b6a43-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="b6a43-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b6a43-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b6a43-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6a43-155">DateTimeOffset</span></span>|<span data-ttu-id="b6a43-156">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="b6a43-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="b6a43-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="b6a43-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="b6a43-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="b6a43-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="b6a43-159">Сведения о портале конечного пользователя используется для синхронизации приложения из магазина корпорации Майкрософт для бизнеса портал Intune компании.</span><span class="sxs-lookup"><span data-stu-id="b6a43-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="b6a43-160">Доступны три варианта, чтобы выбрать нужное \[«Компании только портала», «Компании портала и частных хранилища», «Только для частного хранилища»\].</span><span class="sxs-lookup"><span data-stu-id="b6a43-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="b6a43-161">Возможные значения: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="b6a43-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="b6a43-162">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b6a43-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="b6a43-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a43-163">Response</span></span>
<span data-ttu-id="b6a43-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a43-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a43-165">Пример</span><span class="sxs-lookup"><span data-stu-id="b6a43-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6a43-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a43-166">Request</span></span>

<span data-ttu-id="b6a43-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6a43-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b6a43-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a43-168">Response</span></span>

<span data-ttu-id="b6a43-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6a43-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



