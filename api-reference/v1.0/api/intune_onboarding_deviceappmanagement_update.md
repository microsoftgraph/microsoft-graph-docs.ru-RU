# <a name="update-deviceappmanagement"></a><span data-ttu-id="caf5e-101">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="caf5e-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="caf5e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="caf5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caf5e-103">Обновление свойств объекта [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="caf5e-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caf5e-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="caf5e-104">Prerequisites</span></span>
<span data-ttu-id="caf5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="caf5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="caf5e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caf5e-107">Permission type</span></span>|<span data-ttu-id="caf5e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="caf5e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caf5e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caf5e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="caf5e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf5e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="caf5e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caf5e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caf5e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf5e-112">Not supported.</span></span>|
|<span data-ttu-id="caf5e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caf5e-113">Application</span></span>|<span data-ttu-id="caf5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf5e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caf5e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caf5e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="caf5e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caf5e-116">Request headers</span></span>
|<span data-ttu-id="caf5e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caf5e-117">Header</span></span>|<span data-ttu-id="caf5e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="caf5e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caf5e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf5e-119">Authorization</span></span>|<span data-ttu-id="caf5e-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caf5e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="caf5e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="caf5e-121">Accept</span></span>|<span data-ttu-id="caf5e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="caf5e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caf5e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="caf5e-123">Request body</span></span>
<span data-ttu-id="caf5e-124">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caf5e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="caf5e-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="caf5e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="caf5e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="caf5e-126">Property</span></span>|<span data-ttu-id="caf5e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="caf5e-127">Type</span></span>|<span data-ttu-id="caf5e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="caf5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf5e-129">id</span><span class="sxs-lookup"><span data-stu-id="caf5e-129">id</span></span>|<span data-ttu-id="caf5e-130">String</span><span class="sxs-lookup"><span data-stu-id="caf5e-130">String</span></span>|<span data-ttu-id="caf5e-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="caf5e-131">Not yet documented</span></span>|
|<span data-ttu-id="caf5e-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="caf5e-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="caf5e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf5e-133">DateTimeOffset</span></span>|<span data-ttu-id="caf5e-134">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="caf5e-134">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="caf5e-135">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="caf5e-135">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="caf5e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="caf5e-136">Boolean</span></span>|<span data-ttu-id="caf5e-137">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="caf5e-137">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="caf5e-138">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="caf5e-138">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="caf5e-139">String</span><span class="sxs-lookup"><span data-stu-id="caf5e-139">String</span></span>|<span data-ttu-id="caf5e-140">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="caf5e-140">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="caf5e-141">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="caf5e-141">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="caf5e-142">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="caf5e-142">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="caf5e-143">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="caf5e-143">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="caf5e-144">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="caf5e-144">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="caf5e-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="caf5e-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="caf5e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf5e-146">DateTimeOffset</span></span>|<span data-ttu-id="caf5e-147">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="caf5e-147">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="caf5e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf5e-148">Response</span></span>
<span data-ttu-id="caf5e-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="caf5e-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf5e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="caf5e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="caf5e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="caf5e-151">Request</span></span>
<span data-ttu-id="caf5e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caf5e-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 336

{
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="caf5e-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="caf5e-153">Response</span></span>
<span data-ttu-id="caf5e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="caf5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```



