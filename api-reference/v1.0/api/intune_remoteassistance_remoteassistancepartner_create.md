# <a name="create-remoteassistancepartner"></a><span data-ttu-id="c4fad-101">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="c4fad-101">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="c4fad-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4fad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4fad-103">Создание объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4fad-103">Create a new [plannerBucket](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4fad-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c4fad-104">Prerequisites</span></span>
<span data-ttu-id="c4fad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4fad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c4fad-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4fad-107">Permission type</span></span>|<span data-ttu-id="c4fad-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4fad-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4fad-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4fad-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c4fad-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4fad-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4fad-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4fad-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4fad-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4fad-112">Not supported.</span></span>|
|<span data-ttu-id="c4fad-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4fad-113">Application</span></span>|<span data-ttu-id="c4fad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4fad-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4fad-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4fad-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="c4fad-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4fad-116">Request headers</span></span>
|<span data-ttu-id="c4fad-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4fad-117">Header</span></span>|<span data-ttu-id="c4fad-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c4fad-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4fad-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4fad-119">Authorization</span></span>|<span data-ttu-id="c4fad-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4fad-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4fad-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c4fad-121">Accept</span></span>|<span data-ttu-id="c4fad-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c4fad-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4fad-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4fad-123">Request body</span></span>
<span data-ttu-id="c4fad-124">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4fad-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="c4fad-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="c4fad-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c4fad-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4fad-126">Property</span></span>|<span data-ttu-id="c4fad-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c4fad-127">Type</span></span>|<span data-ttu-id="c4fad-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c4fad-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4fad-129">id</span><span class="sxs-lookup"><span data-stu-id="c4fad-129">id</span></span>|<span data-ttu-id="c4fad-130">String</span><span class="sxs-lookup"><span data-stu-id="c4fad-130">String</span></span>|<span data-ttu-id="c4fad-131">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="c4fad-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="c4fad-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c4fad-132">displayName</span></span>|<span data-ttu-id="c4fad-133">String</span><span class="sxs-lookup"><span data-stu-id="c4fad-133">String</span></span>|<span data-ttu-id="c4fad-134">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="c4fad-134">Display name of the template.</span></span>|
|<span data-ttu-id="c4fad-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="c4fad-135">onboardingUrl</span></span>|<span data-ttu-id="c4fad-136">String</span><span class="sxs-lookup"><span data-stu-id="c4fad-136">String</span></span>|<span data-ttu-id="c4fad-137">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="c4fad-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="c4fad-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c4fad-138">onboardingStatus</span></span>|<span data-ttu-id="c4fad-139">String</span><span class="sxs-lookup"><span data-stu-id="c4fad-139">String</span></span>|<span data-ttu-id="c4fad-140">Подлежит определению. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="c4fad-140">Possible values are: `notOnboarded`, `onboarding`, `onboarded`, .</span></span>|
|<span data-ttu-id="c4fad-141">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c4fad-141">lastConnectionDateTime</span></span>|<span data-ttu-id="c4fad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4fad-142">DateTimeOffset</span></span>|<span data-ttu-id="c4fad-143">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="c4fad-143">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c4fad-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4fad-144">Response</span></span>
<span data-ttu-id="c4fad-145">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4fad-145">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4fad-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c4fad-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4fad-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4fad-147">Request</span></span>
<span data-ttu-id="c4fad-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4fad-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c4fad-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4fad-149">Response</span></span>
<span data-ttu-id="c4fad-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c4fad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



