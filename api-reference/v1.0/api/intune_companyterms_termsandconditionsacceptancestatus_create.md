# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="c5f3f-101">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="c5f3f-101">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="c5f3f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5f3f-103">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c5f3f-103">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5f3f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5f3f-104">Prerequisites</span></span>
<span data-ttu-id="c5f3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5f3f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f3f-107">Permission type</span></span>|<span data-ttu-id="c5f3f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5f3f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f3f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f3f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f3f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f3f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5f3f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f3f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f3f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-112">Not supported.</span></span>|
|<span data-ttu-id="c5f3f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5f3f-113">Application</span></span>|<span data-ttu-id="c5f3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f3f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f3f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c5f3f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5f3f-116">Request headers</span></span>
|<span data-ttu-id="c5f3f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5f3f-117">Header</span></span>|<span data-ttu-id="c5f3f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f3f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f3f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f3f-119">Authorization</span></span>|<span data-ttu-id="c5f3f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f3f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c5f3f-121">Accept</span></span>|<span data-ttu-id="c5f3f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f3f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f3f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f3f-123">Request body</span></span>
<span data-ttu-id="c5f3f-124">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-124">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="c5f3f-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-125">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="c5f3f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f3f-126">Property</span></span>|<span data-ttu-id="c5f3f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f3f-127">Type</span></span>|<span data-ttu-id="c5f3f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f3f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f3f-129">id</span><span class="sxs-lookup"><span data-stu-id="c5f3f-129">id</span></span>|<span data-ttu-id="c5f3f-130">String</span><span class="sxs-lookup"><span data-stu-id="c5f3f-130">String</span></span>|<span data-ttu-id="c5f3f-131">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c5f3f-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5f3f-132">userDisplayName</span></span>|<span data-ttu-id="c5f3f-133">String</span><span class="sxs-lookup"><span data-stu-id="c5f3f-133">String</span></span>|<span data-ttu-id="c5f3f-134">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="c5f3f-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="c5f3f-135">acceptedVersion</span></span>|<span data-ttu-id="c5f3f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f3f-136">Int32</span></span>|<span data-ttu-id="c5f3f-137">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="c5f3f-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f3f-138">acceptedDateTime</span></span>|<span data-ttu-id="c5f3f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f3f-139">DateTimeOffset</span></span>|<span data-ttu-id="c5f3f-140">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="c5f3f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f3f-141">Response</span></span>
<span data-ttu-id="c5f3f-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-142">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f3f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c5f3f-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5f3f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f3f-144">Request</span></span>
<span data-ttu-id="c5f3f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c5f3f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f3f-146">Response</span></span>
<span data-ttu-id="c5f3f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5f3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



