# <a name="delete-targetedmanagedapppolicyassignment"></a><span data-ttu-id="6bcab-101">Удаление targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6bcab-101">Delete targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="6bcab-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bcab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bcab-103">Удаляет объект [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6bcab-103">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bcab-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6bcab-104">Prerequisites</span></span>
<span data-ttu-id="6bcab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6bcab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6bcab-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="6bcab-107">Permission type</span></span>|<span data-ttu-id="6bcab-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bcab-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bcab-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bcab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6bcab-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bcab-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6bcab-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bcab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bcab-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bcab-112">Not supported.</span></span>|
|<span data-ttu-id="6bcab-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bcab-113">Application</span></span>|<span data-ttu-id="6bcab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bcab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bcab-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bcab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6bcab-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bcab-116">Request headers</span></span>
|<span data-ttu-id="6bcab-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bcab-117">Header</span></span>|<span data-ttu-id="6bcab-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6bcab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bcab-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bcab-119">Authorization</span></span>|<span data-ttu-id="6bcab-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bcab-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bcab-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6bcab-121">Accept</span></span>|<span data-ttu-id="6bcab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6bcab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bcab-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bcab-123">Request body</span></span>
<span data-ttu-id="6bcab-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bcab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bcab-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bcab-125">Response</span></span>
<span data-ttu-id="6bcab-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6bcab-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6bcab-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6bcab-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bcab-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bcab-128">Request</span></span>
<span data-ttu-id="6bcab-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bcab-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6bcab-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bcab-130">Response</span></span>
<span data-ttu-id="6bcab-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6bcab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



