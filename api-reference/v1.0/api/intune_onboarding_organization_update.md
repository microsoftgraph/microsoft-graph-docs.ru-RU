# <a name="update-organization"></a><span data-ttu-id="97c1f-101">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="97c1f-101">Update organization</span></span>

> <span data-ttu-id="97c1f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97c1f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97c1f-103">Обновление свойств объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="97c1f-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97c1f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="97c1f-104">Prerequisites</span></span>
<span data-ttu-id="97c1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97c1f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97c1f-107">Permission type</span></span>|<span data-ttu-id="97c1f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97c1f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97c1f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97c1f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97c1f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97c1f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97c1f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97c1f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97c1f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97c1f-112">Not supported.</span></span>|
|<span data-ttu-id="97c1f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97c1f-113">Application</span></span>|<span data-ttu-id="97c1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97c1f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97c1f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97c1f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="97c1f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97c1f-116">Request headers</span></span>
|<span data-ttu-id="97c1f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97c1f-117">Header</span></span>|<span data-ttu-id="97c1f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="97c1f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97c1f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="97c1f-119">Authorization</span></span>|<span data-ttu-id="97c1f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97c1f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97c1f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="97c1f-121">Accept</span></span>|<span data-ttu-id="97c1f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97c1f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97c1f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97c1f-123">Request body</span></span>
<span data-ttu-id="97c1f-124">В теле запроса добавьте представление объекта [organization](../resources/intune_onboarding_organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97c1f-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="97c1f-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="97c1f-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="97c1f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="97c1f-126">Property</span></span>|<span data-ttu-id="97c1f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="97c1f-127">Type</span></span>|<span data-ttu-id="97c1f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="97c1f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c1f-129">id</span><span class="sxs-lookup"><span data-stu-id="97c1f-129">id</span></span>|<span data-ttu-id="97c1f-130">String</span><span class="sxs-lookup"><span data-stu-id="97c1f-130">String</span></span>|<span data-ttu-id="97c1f-131">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="97c1f-131">The GUID for the object.</span></span>|
|<span data-ttu-id="97c1f-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="97c1f-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="97c1f-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="97c1f-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="97c1f-134">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="97c1f-134">Mobile device management authority.</span></span> <span data-ttu-id="97c1f-135">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="97c1f-135">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="97c1f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="97c1f-136">Response</span></span>
<span data-ttu-id="97c1f-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune_onboarding_organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="97c1f-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97c1f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="97c1f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="97c1f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="97c1f-139">Request</span></span>
<span data-ttu-id="97c1f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97c1f-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="97c1f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="97c1f-141">Response</span></span>
<span data-ttu-id="97c1f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="97c1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



