# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="79873-101">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="79873-101">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="79873-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79873-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79873-103">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="79873-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79873-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79873-104">Prerequisites</span></span>
<span data-ttu-id="79873-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79873-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79873-107">Permission type</span></span>|<span data-ttu-id="79873-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79873-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79873-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79873-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79873-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79873-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79873-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79873-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79873-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79873-112">Not supported.</span></span>|
|<span data-ttu-id="79873-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79873-113">Application</span></span>|<span data-ttu-id="79873-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79873-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79873-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79873-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="79873-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79873-116">Request headers</span></span>
|<span data-ttu-id="79873-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79873-117">Header</span></span>|<span data-ttu-id="79873-118">Значение</span><span class="sxs-lookup"><span data-stu-id="79873-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79873-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="79873-119">Authorization</span></span>|<span data-ttu-id="79873-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79873-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79873-121">Accept</span><span class="sxs-lookup"><span data-stu-id="79873-121">Accept</span></span>|<span data-ttu-id="79873-122">application/json</span><span class="sxs-lookup"><span data-stu-id="79873-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79873-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79873-123">Request body</span></span>
<span data-ttu-id="79873-124">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79873-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="79873-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="79873-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="79873-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="79873-126">Property</span></span>|<span data-ttu-id="79873-127">Тип</span><span class="sxs-lookup"><span data-stu-id="79873-127">Type</span></span>|<span data-ttu-id="79873-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79873-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79873-129">displayName</span><span class="sxs-lookup"><span data-stu-id="79873-129">displayName</span></span>|<span data-ttu-id="79873-130">String</span><span class="sxs-lookup"><span data-stu-id="79873-130">String</span></span>|<span data-ttu-id="79873-131">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="79873-131">The friendly name</span></span>|
|<span data-ttu-id="79873-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="79873-132">fileHash</span></span>|<span data-ttu-id="79873-133">String</span><span class="sxs-lookup"><span data-stu-id="79873-133">String</span></span>|<span data-ttu-id="79873-134">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="79873-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="79873-135">file</span><span class="sxs-lookup"><span data-stu-id="79873-135">file</span></span>|<span data-ttu-id="79873-136">Binary</span><span class="sxs-lookup"><span data-stu-id="79873-136">Binary</span></span>|<span data-ttu-id="79873-137">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="79873-137">File as a byte array</span></span>|
|<span data-ttu-id="79873-138">id</span><span class="sxs-lookup"><span data-stu-id="79873-138">id</span></span>|<span data-ttu-id="79873-139">String</span><span class="sxs-lookup"><span data-stu-id="79873-139">String</span></span>|<span data-ttu-id="79873-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79873-140">Key of the setting.</span></span>|
|<span data-ttu-id="79873-141">version</span><span class="sxs-lookup"><span data-stu-id="79873-141">version</span></span>|<span data-ttu-id="79873-142">String</span><span class="sxs-lookup"><span data-stu-id="79873-142">String</span></span>|<span data-ttu-id="79873-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="79873-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="79873-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="79873-144">Response</span></span>
<span data-ttu-id="79873-145">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79873-145">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79873-146">Пример</span><span class="sxs-lookup"><span data-stu-id="79873-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="79873-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="79873-147">Request</span></span>
<span data-ttu-id="79873-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79873-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="79873-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="79873-149">Response</span></span>
<span data-ttu-id="79873-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79873-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



