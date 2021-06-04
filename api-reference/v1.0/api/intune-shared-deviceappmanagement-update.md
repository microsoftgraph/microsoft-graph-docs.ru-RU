---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 419bdc52dd9dbc7b67528b4a8b109bb309547f95
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732950"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="9d7f9-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9d7f9-103">Update deviceAppManagement</span></span>

<span data-ttu-id="9d7f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d7f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d7f9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d7f9-106">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9d7f9-106">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d7f9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d7f9-107">Prerequisites</span></span>
<span data-ttu-id="9d7f9-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9d7f9-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d7f9-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9d7f9-110">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="9d7f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d7f9-111">Permission type</span></span>|<span data-ttu-id="9d7f9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d7f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d7f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d7f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d7f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d7f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d7f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d7f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d7f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-116">Not supported.</span></span>|
|<span data-ttu-id="9d7f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d7f9-117">Application</span></span>|<span data-ttu-id="9d7f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d7f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d7f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="9d7f9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d7f9-120">Request headers</span></span>
|<span data-ttu-id="9d7f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d7f9-121">Header</span></span>|<span data-ttu-id="9d7f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d7f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d7f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d7f9-123">Authorization</span></span>|<span data-ttu-id="9d7f9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d7f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d7f9-125">Accept</span></span>|<span data-ttu-id="9d7f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d7f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d7f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d7f9-127">Request body</span></span>
<span data-ttu-id="9d7f9-128">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-128">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="9d7f9-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9d7f9-129">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="9d7f9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d7f9-130">Property</span></span>|<span data-ttu-id="9d7f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d7f9-131">Type</span></span>|<span data-ttu-id="9d7f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d7f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d7f9-133">id</span><span class="sxs-lookup"><span data-stu-id="9d7f9-133">id</span></span>|<span data-ttu-id="9d7f9-134">String</span><span class="sxs-lookup"><span data-stu-id="9d7f9-134">String</span></span>|<span data-ttu-id="9d7f9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-135">Key of the entity.</span></span>|
|<span data-ttu-id="9d7f9-136">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="9d7f9-136">**Onboarding**</span></span>|
|<span data-ttu-id="9d7f9-137">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="9d7f9-137">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="9d7f9-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d7f9-138">Boolean</span></span>|<span data-ttu-id="9d7f9-139">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-139">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="9d7f9-140">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="9d7f9-140">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="9d7f9-141">String</span><span class="sxs-lookup"><span data-stu-id="9d7f9-141">String</span></span>|<span data-ttu-id="9d7f9-142">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-142">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="9d7f9-143">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-143">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="9d7f9-144">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9d7f9-144">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="9d7f9-145">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-145">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="9d7f9-146">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-146">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="9d7f9-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="9d7f9-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="9d7f9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d7f9-148">DateTimeOffset</span></span>|<span data-ttu-id="9d7f9-149">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-149">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="9d7f9-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9d7f9-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9d7f9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d7f9-151">DateTimeOffset</span></span>|<span data-ttu-id="9d7f9-152">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-152">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="9d7f9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d7f9-153">Response</span></span>
<span data-ttu-id="9d7f9-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-154">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="9d7f9-155">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="9d7f9-155">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="9d7f9-156">Пример отклика</span><span class="sxs-lookup"><span data-stu-id="9d7f9-156">Example response</span></span>

<span data-ttu-id="9d7f9-157">Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-157">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d7f9-158">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d7f9-158">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









