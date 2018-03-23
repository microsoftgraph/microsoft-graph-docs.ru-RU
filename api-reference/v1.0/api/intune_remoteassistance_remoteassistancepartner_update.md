# <a name="update-remoteassistancepartner"></a><span data-ttu-id="21131-101">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="21131-101">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="21131-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21131-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21131-103">Обновление свойств объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="21131-103">Update the properties of a [calendar](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21131-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21131-104">Prerequisites</span></span>
<span data-ttu-id="21131-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="21131-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21131-107">Permission type</span></span>|<span data-ttu-id="21131-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21131-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21131-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21131-109">Delegated (work or school account)</span></span>|<span data-ttu-id="21131-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21131-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21131-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21131-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21131-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21131-112">Not supported.</span></span>|
|<span data-ttu-id="21131-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21131-113">Application</span></span>|<span data-ttu-id="21131-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21131-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21131-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21131-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="21131-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21131-116">Request headers</span></span>
|<span data-ttu-id="21131-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21131-117">Header</span></span>|<span data-ttu-id="21131-118">Значение</span><span class="sxs-lookup"><span data-stu-id="21131-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21131-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="21131-119">Authorization</span></span>|<span data-ttu-id="21131-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21131-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="21131-121">Accept</span><span class="sxs-lookup"><span data-stu-id="21131-121">Accept</span></span>|<span data-ttu-id="21131-122">application/json</span><span class="sxs-lookup"><span data-stu-id="21131-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21131-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21131-123">Request body</span></span>
<span data-ttu-id="21131-124">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21131-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="21131-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="21131-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="21131-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="21131-126">Property</span></span>|<span data-ttu-id="21131-127">Тип</span><span class="sxs-lookup"><span data-stu-id="21131-127">Type</span></span>|<span data-ttu-id="21131-128">Описание</span><span class="sxs-lookup"><span data-stu-id="21131-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21131-129">id</span><span class="sxs-lookup"><span data-stu-id="21131-129">id</span></span>|<span data-ttu-id="21131-130">String</span><span class="sxs-lookup"><span data-stu-id="21131-130">String</span></span>|<span data-ttu-id="21131-131">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="21131-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="21131-132">displayName</span><span class="sxs-lookup"><span data-stu-id="21131-132">displayName</span></span>|<span data-ttu-id="21131-133">String</span><span class="sxs-lookup"><span data-stu-id="21131-133">String</span></span>|<span data-ttu-id="21131-134">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="21131-134">Display name of the template.</span></span>|
|<span data-ttu-id="21131-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="21131-135">onboardingUrl</span></span>|<span data-ttu-id="21131-136">String</span><span class="sxs-lookup"><span data-stu-id="21131-136">String</span></span>|<span data-ttu-id="21131-137">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="21131-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="21131-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="21131-138">onboardingStatus</span></span>|<span data-ttu-id="21131-139">String</span><span class="sxs-lookup"><span data-stu-id="21131-139">String</span></span>|<span data-ttu-id="21131-140">Подлежит определению. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="21131-140">Possible values are: `notOnboarded`, `onboarding`, `onboarded`, .</span></span>|
|<span data-ttu-id="21131-141">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="21131-141">lastConnectionDateTime</span></span>|<span data-ttu-id="21131-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21131-142">DateTimeOffset</span></span>|<span data-ttu-id="21131-143">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="21131-143">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="21131-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="21131-144">Response</span></span>
<span data-ttu-id="21131-145">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21131-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21131-146">Пример</span><span class="sxs-lookup"><span data-stu-id="21131-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="21131-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="21131-147">Request</span></span>
<span data-ttu-id="21131-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21131-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="21131-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="21131-149">Response</span></span>
<span data-ttu-id="21131-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21131-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



