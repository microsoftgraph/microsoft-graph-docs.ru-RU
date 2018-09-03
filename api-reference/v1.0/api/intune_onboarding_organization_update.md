# <a name="update-organization"></a><span data-ttu-id="dccfa-101">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="dccfa-101">Update organization</span></span>

> <span data-ttu-id="dccfa-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dccfa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dccfa-103">Обновление свойств объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="dccfa-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dccfa-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dccfa-104">Prerequisites</span></span>
<span data-ttu-id="dccfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dccfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dccfa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dccfa-107">Permission type</span></span>|<span data-ttu-id="dccfa-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dccfa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dccfa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dccfa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dccfa-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dccfa-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dccfa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dccfa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dccfa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dccfa-112">Not supported.</span></span>|
|<span data-ttu-id="dccfa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dccfa-113">Application</span></span>|<span data-ttu-id="dccfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dccfa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dccfa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dccfa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="dccfa-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dccfa-116">Request headers</span></span>
|<span data-ttu-id="dccfa-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dccfa-117">Header</span></span>|<span data-ttu-id="dccfa-118">Значение</span><span class="sxs-lookup"><span data-stu-id="dccfa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dccfa-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dccfa-119">Authorization</span></span>|<span data-ttu-id="dccfa-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="dccfa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dccfa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="dccfa-121">Accept</span></span>|<span data-ttu-id="dccfa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dccfa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dccfa-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dccfa-123">Request body</span></span>
<span data-ttu-id="dccfa-124">В теле запроса добавьте представление объекта [organization](../resources/intune_onboarding_organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dccfa-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="dccfa-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="dccfa-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="dccfa-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="dccfa-126">Property</span></span>|<span data-ttu-id="dccfa-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dccfa-127">Type</span></span>|<span data-ttu-id="dccfa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dccfa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dccfa-129">id</span><span class="sxs-lookup"><span data-stu-id="dccfa-129">id</span></span>|<span data-ttu-id="dccfa-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="dccfa-130">String</span></span>|<span data-ttu-id="dccfa-131">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="dccfa-131">The GUID for the object.</span></span>|
|<span data-ttu-id="dccfa-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="dccfa-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="dccfa-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="dccfa-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="dccfa-134">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="dccfa-134">Mobile device management authority.</span></span> <span data-ttu-id="dccfa-135">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="dccfa-135">The possible values are `unknown`, `intune`, `sccm`, `office365`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="dccfa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dccfa-136">Response</span></span>
<span data-ttu-id="dccfa-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune_onboarding_organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dccfa-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dccfa-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dccfa-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="dccfa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="dccfa-139">Request</span></span>
<span data-ttu-id="dccfa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dccfa-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="dccfa-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="dccfa-141">Response</span></span>
<span data-ttu-id="dccfa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dccfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



