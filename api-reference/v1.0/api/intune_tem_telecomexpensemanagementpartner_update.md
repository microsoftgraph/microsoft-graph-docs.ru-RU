# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="f40bf-101">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="f40bf-101">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="f40bf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f40bf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f40bf-103">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="f40bf-103">Update the properties of a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f40bf-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f40bf-104">Prerequisites</span></span>
<span data-ttu-id="f40bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f40bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f40bf-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f40bf-107">Permission type</span></span>|<span data-ttu-id="f40bf-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f40bf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f40bf-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f40bf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f40bf-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f40bf-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f40bf-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f40bf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f40bf-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f40bf-112">Not supported.</span></span>|
|<span data-ttu-id="f40bf-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f40bf-113">Application</span></span>|<span data-ttu-id="f40bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f40bf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f40bf-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f40bf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="f40bf-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f40bf-116">Request headers</span></span>
|<span data-ttu-id="f40bf-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f40bf-117">Header</span></span>|<span data-ttu-id="f40bf-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f40bf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f40bf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f40bf-119">Authorization</span></span>|<span data-ttu-id="f40bf-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f40bf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f40bf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f40bf-121">Accept</span></span>|<span data-ttu-id="f40bf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f40bf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f40bf-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f40bf-123">Request body</span></span>
<span data-ttu-id="f40bf-124">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f40bf-124">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="f40bf-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="f40bf-125">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="f40bf-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f40bf-126">Property</span></span>|<span data-ttu-id="f40bf-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f40bf-127">Type</span></span>|<span data-ttu-id="f40bf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f40bf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f40bf-129">id</span><span class="sxs-lookup"><span data-stu-id="f40bf-129">id</span></span>|<span data-ttu-id="f40bf-130">String</span><span class="sxs-lookup"><span data-stu-id="f40bf-130">String</span></span>|<span data-ttu-id="f40bf-131">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="f40bf-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="f40bf-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f40bf-132">displayName</span></span>|<span data-ttu-id="f40bf-133">String</span><span class="sxs-lookup"><span data-stu-id="f40bf-133">String</span></span>|<span data-ttu-id="f40bf-134">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="f40bf-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="f40bf-135">url</span><span class="sxs-lookup"><span data-stu-id="f40bf-135">url</span></span>|<span data-ttu-id="f40bf-136">String</span><span class="sxs-lookup"><span data-stu-id="f40bf-136">String</span></span>|<span data-ttu-id="f40bf-137">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="f40bf-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="f40bf-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="f40bf-138">appAuthorized</span></span>|<span data-ttu-id="f40bf-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f40bf-139">Boolean</span></span>|<span data-ttu-id="f40bf-140">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="f40bf-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="f40bf-141">enabled</span><span class="sxs-lookup"><span data-stu-id="f40bf-141">enabled</span></span>|<span data-ttu-id="f40bf-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f40bf-142">Boolean</span></span>|<span data-ttu-id="f40bf-143">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="f40bf-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="f40bf-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f40bf-144">lastConnectionDateTime</span></span>|<span data-ttu-id="f40bf-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f40bf-145">DateTimeOffset</span></span>|<span data-ttu-id="f40bf-146">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="f40bf-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="f40bf-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f40bf-147">Response</span></span>
<span data-ttu-id="f40bf-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f40bf-148">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f40bf-149">Пример</span><span class="sxs-lookup"><span data-stu-id="f40bf-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="f40bf-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f40bf-150">Request</span></span>
<span data-ttu-id="f40bf-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f40bf-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f40bf-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="f40bf-152">Response</span></span>
<span data-ttu-id="f40bf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f40bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



