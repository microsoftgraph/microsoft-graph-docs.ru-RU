# <a name="update-deviceappmanagement"></a><span data-ttu-id="7114d-101">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7114d-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="7114d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7114d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7114d-103">Обновление свойств объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7114d-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7114d-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="7114d-104">Prerequisites</span></span>
<span data-ttu-id="7114d-105">Чтобы вызвать этот API, необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="7114d-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="7114d-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7114d-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="7114d-107">Обратите внимание на то, что соответствующее разрешение изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="7114d-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="7114d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7114d-108">Permission type</span></span>|<span data-ttu-id="7114d-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7114d-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7114d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7114d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7114d-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7114d-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7114d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7114d-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7114d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7114d-113">Not supported.</span></span>|
|<span data-ttu-id="7114d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7114d-114">Application</span></span>|<span data-ttu-id="7114d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7114d-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7114d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7114d-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="7114d-117">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7114d-117">Request headers</span></span>
|<span data-ttu-id="7114d-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7114d-118">Header</span></span>|<span data-ttu-id="7114d-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7114d-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7114d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7114d-120">Authorization</span></span>|<span data-ttu-id="7114d-121">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7114d-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7114d-122">Accept</span><span class="sxs-lookup"><span data-stu-id="7114d-122">Accept</span></span>|<span data-ttu-id="7114d-123">application/json</span><span class="sxs-lookup"><span data-stu-id="7114d-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7114d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7114d-124">Request body</span></span>
<span data-ttu-id="7114d-125">В теле запроса добавьте представление объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7114d-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="7114d-126">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7114d-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="7114d-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="7114d-127">Property</span></span>|<span data-ttu-id="7114d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7114d-128">Type</span></span>|<span data-ttu-id="7114d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7114d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7114d-130">id</span><span class="sxs-lookup"><span data-stu-id="7114d-130">id</span></span>|<span data-ttu-id="7114d-131">string</span><span class="sxs-lookup"><span data-stu-id="7114d-131">String</span></span>|<span data-ttu-id="7114d-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7114d-132">Key of the entity.</span></span>|
|<span data-ttu-id="7114d-133">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7114d-133">**On-boarding**</span></span>|
|<span data-ttu-id="7114d-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="7114d-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="7114d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7114d-135">Boolean</span></span>|<span data-ttu-id="7114d-136">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7114d-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="7114d-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="7114d-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="7114d-138">string</span><span class="sxs-lookup"><span data-stu-id="7114d-138">String</span></span>|<span data-ttu-id="7114d-139">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7114d-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="7114d-140">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="7114d-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="7114d-141">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="7114d-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="7114d-142">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="7114d-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="7114d-143">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="7114d-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="7114d-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="7114d-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="7114d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7114d-145">DateTimeOffset</span></span>|<span data-ttu-id="7114d-146">Время выполнения последней синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7114d-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="7114d-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7114d-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7114d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7114d-148">DateTimeOffset</span></span>|<span data-ttu-id="7114d-149">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7114d-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="7114d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7114d-150">Response</span></span>
<span data-ttu-id="7114d-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7114d-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="7114d-152">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="7114d-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="7114d-153">Пример отклика</span><span class="sxs-lookup"><span data-stu-id="7114d-153">Example response</span></span>

<span data-ttu-id="7114d-154">Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="7114d-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7114d-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7114d-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



