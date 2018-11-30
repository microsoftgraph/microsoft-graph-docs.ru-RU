---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
ms.openlocfilehash: 92d792f0ee4bab4923eda03cd488ece0a75f8ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027497"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="e3c86-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="e3c86-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="e3c86-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3c86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3c86-105">Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e3c86-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3c86-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3c86-106">Prerequisites</span></span>
<span data-ttu-id="e3c86-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e3c86-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e3c86-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c86-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e3c86-109">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="e3c86-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="e3c86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3c86-110">Permission type</span></span>|<span data-ttu-id="e3c86-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3c86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3c86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3c86-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c86-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3c86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3c86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3c86-115">Not supported.</span></span>|
|<span data-ttu-id="e3c86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3c86-116">Application</span></span>|<span data-ttu-id="e3c86-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3c86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3c86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="e3c86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3c86-119">Request headers</span></span>
|<span data-ttu-id="e3c86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3c86-120">Header</span></span>|<span data-ttu-id="e3c86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e3c86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3c86-122">Authorization</span></span>|<span data-ttu-id="e3c86-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3c86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e3c86-124">Accept</span></span>|<span data-ttu-id="e3c86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3c86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c86-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3c86-126">Request body</span></span>
<span data-ttu-id="e3c86-127">В теле запроса добавьте представление объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3c86-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="e3c86-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e3c86-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="e3c86-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3c86-129">Property</span></span>|<span data-ttu-id="e3c86-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e3c86-130">Type</span></span>|<span data-ttu-id="e3c86-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c86-132">id</span><span class="sxs-lookup"><span data-stu-id="e3c86-132">id</span></span>|<span data-ttu-id="e3c86-133">String</span><span class="sxs-lookup"><span data-stu-id="e3c86-133">String</span></span>|<span data-ttu-id="e3c86-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3c86-134">Key of the entity.</span></span>|
|<span data-ttu-id="e3c86-135">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="e3c86-135">**Onboarding**</span></span>|
|<span data-ttu-id="e3c86-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="e3c86-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="e3c86-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3c86-137">Boolean</span></span>|<span data-ttu-id="e3c86-138">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e3c86-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="e3c86-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="e3c86-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="e3c86-140">String</span><span class="sxs-lookup"><span data-stu-id="e3c86-140">String</span></span>|<span data-ttu-id="e3c86-141">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e3c86-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="e3c86-142">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="e3c86-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="e3c86-143">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="e3c86-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="e3c86-144">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="e3c86-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="e3c86-145">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="e3c86-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="e3c86-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="e3c86-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="e3c86-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c86-147">DateTimeOffset</span></span>|<span data-ttu-id="e3c86-148">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e3c86-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="e3c86-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c86-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="e3c86-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c86-150">DateTimeOffset</span></span>|<span data-ttu-id="e3c86-151">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="e3c86-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="e3c86-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3c86-152">Response</span></span>
<span data-ttu-id="e3c86-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3c86-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="e3c86-154">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="e3c86-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="e3c86-155">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="e3c86-155">Example response</span></span>

<span data-ttu-id="e3c86-156">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e3c86-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3c86-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3c86-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



