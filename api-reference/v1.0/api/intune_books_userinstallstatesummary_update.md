# <a name="update-userinstallstatesummary"></a><span data-ttu-id="e792f-101">Обновление объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e792f-101">Update userInstallStateSummary</span></span>

> <span data-ttu-id="e792f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e792f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e792f-103">Обновление свойств объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e792f-103">Update the properties of a [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e792f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e792f-104">Prerequisites</span></span>
<span data-ttu-id="e792f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e792f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e792f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e792f-107">Permission type</span></span>|<span data-ttu-id="e792f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e792f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e792f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e792f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e792f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e792f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e792f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e792f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e792f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e792f-112">Not supported.</span></span>|
|<span data-ttu-id="e792f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e792f-113">Application</span></span>|<span data-ttu-id="e792f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e792f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e792f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e792f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e792f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e792f-116">Request headers</span></span>
|<span data-ttu-id="e792f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e792f-117">Header</span></span>|<span data-ttu-id="e792f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e792f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e792f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e792f-119">Authorization</span></span>|<span data-ttu-id="e792f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e792f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e792f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e792f-121">Accept</span></span>|<span data-ttu-id="e792f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e792f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e792f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e792f-123">Request body</span></span>
<span data-ttu-id="e792f-124">В тексте запроса добавьте представление объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e792f-124">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="e792f-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e792f-125">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span></span>

|<span data-ttu-id="e792f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e792f-126">Property</span></span>|<span data-ttu-id="e792f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e792f-127">Type</span></span>|<span data-ttu-id="e792f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e792f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e792f-129">id</span><span class="sxs-lookup"><span data-stu-id="e792f-129">id</span></span>|<span data-ttu-id="e792f-130">String</span><span class="sxs-lookup"><span data-stu-id="e792f-130">String</span></span>|<span data-ttu-id="e792f-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e792f-131">Key of the entity.</span></span>|
|<span data-ttu-id="e792f-132">userName</span><span class="sxs-lookup"><span data-stu-id="e792f-132">userName</span></span>|<span data-ttu-id="e792f-133">String</span><span class="sxs-lookup"><span data-stu-id="e792f-133">String</span></span>|<span data-ttu-id="e792f-134">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e792f-134">User name.</span></span>|
|<span data-ttu-id="e792f-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e792f-135">installedDeviceCount</span></span>|<span data-ttu-id="e792f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e792f-136">Int32</span></span>|<span data-ttu-id="e792f-137">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e792f-137">Installed Device Count.</span></span>|
|<span data-ttu-id="e792f-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e792f-138">failedDeviceCount</span></span>|<span data-ttu-id="e792f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e792f-139">Int32</span></span>|<span data-ttu-id="e792f-140">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="e792f-140">Failed Device Count.</span></span>|
|<span data-ttu-id="e792f-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e792f-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="e792f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e792f-142">Int32</span></span>|<span data-ttu-id="e792f-143">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e792f-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="e792f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e792f-144">Response</span></span>
<span data-ttu-id="e792f-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e792f-145">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e792f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="e792f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e792f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e792f-147">Request</span></span>
<span data-ttu-id="e792f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e792f-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="e792f-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="e792f-149">Response</span></span>
<span data-ttu-id="e792f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e792f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



