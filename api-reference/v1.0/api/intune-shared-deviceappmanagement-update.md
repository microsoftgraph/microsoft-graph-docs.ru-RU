---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97316e06cec39cd0aeb1b22d6142925d81b77ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577072"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="a4589-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a4589-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="a4589-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4589-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4589-105">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a4589-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4589-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4589-106">Prerequisites</span></span>
<span data-ttu-id="a4589-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a4589-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a4589-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4589-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="a4589-109">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="a4589-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="a4589-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4589-110">Permission type</span></span>|<span data-ttu-id="a4589-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4589-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4589-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4589-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4589-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4589-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4589-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4589-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4589-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4589-115">Not supported.</span></span>|
|<span data-ttu-id="a4589-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4589-116">Application</span></span>|<span data-ttu-id="a4589-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4589-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4589-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4589-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="a4589-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4589-119">Request headers</span></span>
|<span data-ttu-id="a4589-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4589-120">Header</span></span>|<span data-ttu-id="a4589-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4589-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4589-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4589-122">Authorization</span></span>|<span data-ttu-id="a4589-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4589-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4589-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4589-124">Accept</span></span>|<span data-ttu-id="a4589-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4589-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4589-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4589-126">Request body</span></span>
<span data-ttu-id="a4589-127">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4589-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="a4589-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a4589-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="a4589-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4589-129">Property</span></span>|<span data-ttu-id="a4589-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4589-130">Type</span></span>|<span data-ttu-id="a4589-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4589-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4589-132">id</span><span class="sxs-lookup"><span data-stu-id="a4589-132">id</span></span>|<span data-ttu-id="a4589-133">String</span><span class="sxs-lookup"><span data-stu-id="a4589-133">String</span></span>|<span data-ttu-id="a4589-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4589-134">Key of the entity.</span></span>|
|<span data-ttu-id="a4589-135">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="a4589-135">**Onboarding**</span></span>|
|<span data-ttu-id="a4589-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="a4589-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="a4589-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4589-137">Boolean</span></span>|<span data-ttu-id="a4589-138">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a4589-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="a4589-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="a4589-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="a4589-140">String</span><span class="sxs-lookup"><span data-stu-id="a4589-140">String</span></span>|<span data-ttu-id="a4589-141">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a4589-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="a4589-142">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="a4589-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="a4589-143">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a4589-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="a4589-144">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="a4589-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="a4589-145">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="a4589-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="a4589-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="a4589-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="a4589-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4589-147">DateTimeOffset</span></span>|<span data-ttu-id="a4589-148">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a4589-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="a4589-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a4589-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a4589-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4589-150">DateTimeOffset</span></span>|<span data-ttu-id="a4589-151">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="a4589-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="a4589-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4589-152">Response</span></span>
<span data-ttu-id="a4589-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4589-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="a4589-154">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="a4589-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="a4589-155">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="a4589-155">Example response</span></span>

<span data-ttu-id="a4589-156">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a4589-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a4589-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4589-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



