# <a name="update-androidforworksettings"></a><span data-ttu-id="68095-101">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="68095-101">Update androidForWorkSettings</span></span>

> <span data-ttu-id="68095-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68095-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68095-103">Обновление свойств объекта [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="68095-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68095-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="68095-104">Prerequisites</span></span>
<span data-ttu-id="68095-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68095-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68095-107">Permission type</span></span>|<span data-ttu-id="68095-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68095-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68095-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68095-109">Delegated (work or school account)</span></span>|<span data-ttu-id="68095-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68095-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68095-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68095-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68095-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68095-112">Not supported.</span></span>|
|<span data-ttu-id="68095-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68095-113">Application</span></span>|<span data-ttu-id="68095-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68095-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68095-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68095-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="68095-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68095-116">Request headers</span></span>
|<span data-ttu-id="68095-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68095-117">Header</span></span>|<span data-ttu-id="68095-118">Значение</span><span class="sxs-lookup"><span data-stu-id="68095-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68095-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="68095-119">Authorization</span></span>|<span data-ttu-id="68095-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68095-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68095-121">Accept</span><span class="sxs-lookup"><span data-stu-id="68095-121">Accept</span></span>|<span data-ttu-id="68095-122">application/json</span><span class="sxs-lookup"><span data-stu-id="68095-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68095-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68095-123">Request body</span></span>
<span data-ttu-id="68095-124">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68095-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>

<span data-ttu-id="68095-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="68095-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="68095-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="68095-126">Property</span></span>|<span data-ttu-id="68095-127">Тип</span><span class="sxs-lookup"><span data-stu-id="68095-127">Type</span></span>|<span data-ttu-id="68095-128">Описание</span><span class="sxs-lookup"><span data-stu-id="68095-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68095-129">id</span><span class="sxs-lookup"><span data-stu-id="68095-129">id</span></span>|<span data-ttu-id="68095-130">String</span><span class="sxs-lookup"><span data-stu-id="68095-130">String</span></span>|<span data-ttu-id="68095-131">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="68095-131">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="68095-132">bindStatus</span><span class="sxs-lookup"><span data-stu-id="68095-132">bindStatus</span></span>|<span data-ttu-id="68095-133">String</span><span class="sxs-lookup"><span data-stu-id="68095-133">String</span></span>|<span data-ttu-id="68095-134">Состояние привязки клиента к API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="68095-134">Bind status of the tenant with the Google EMM API Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="68095-135">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="68095-135">lastAppSyncDateTime</span></span>|<span data-ttu-id="68095-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68095-136">DateTimeOffset</span></span>|<span data-ttu-id="68095-137">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="68095-137">Last completion time for app sync</span></span>|
|<span data-ttu-id="68095-138">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="68095-138">lastAppSyncStatus</span></span>|<span data-ttu-id="68095-139">String</span><span class="sxs-lookup"><span data-stu-id="68095-139">String</span></span>|<span data-ttu-id="68095-140">Результат последней синхронизации приложения. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="68095-140">Last application sync result Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="68095-141">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="68095-141">ownerUserPrincipalName</span></span>|<span data-ttu-id="68095-142">String</span><span class="sxs-lookup"><span data-stu-id="68095-142">String</span></span>|<span data-ttu-id="68095-143">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="68095-143">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="68095-144">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="68095-144">ownerOrganizationName</span></span>|<span data-ttu-id="68095-145">String</span><span class="sxs-lookup"><span data-stu-id="68095-145">String</span></span>|<span data-ttu-id="68095-146">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="68095-146">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="68095-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68095-147">lastModifiedDateTime</span></span>|<span data-ttu-id="68095-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68095-148">DateTimeOffset</span></span>|<span data-ttu-id="68095-149">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="68095-149">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="68095-150">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="68095-150">enrollmentTarget</span></span>|<span data-ttu-id="68095-151">String</span><span class="sxs-lookup"><span data-stu-id="68095-151">String</span></span>|<span data-ttu-id="68095-152">Указывает, какие пользователи могут регистрировать устройства для управления с помощью Android for Work. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="68095-152">Indicates which users can enroll devices in Android for Work device management Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="68095-153">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="68095-153">targetGroupIds</span></span>|<span data-ttu-id="68095-154">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="68095-154">String collection</span></span>|<span data-ttu-id="68095-155">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="68095-155">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|



## <a name="response"></a><span data-ttu-id="68095-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="68095-156">Response</span></span>
<span data-ttu-id="68095-157">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68095-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68095-158">Пример</span><span class="sxs-lookup"><span data-stu-id="68095-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="68095-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="68095-159">Request</span></span>
<span data-ttu-id="68095-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68095-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="68095-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="68095-161">Response</span></span>
<span data-ttu-id="68095-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="68095-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



