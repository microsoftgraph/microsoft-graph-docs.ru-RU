# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="c6af4-101">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="c6af4-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="c6af4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6af4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6af4-103">Обновляет свойства объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="c6af4-103">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6af4-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6af4-104">Prerequisites</span></span>
<span data-ttu-id="c6af4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6af4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c6af4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6af4-107">Permission type</span></span>|<span data-ttu-id="c6af4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6af4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6af4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6af4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c6af4-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6af4-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6af4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6af4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6af4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6af4-112">Not supported.</span></span>|
|<span data-ttu-id="c6af4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6af4-113">Application</span></span>|<span data-ttu-id="c6af4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6af4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6af4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6af4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="c6af4-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6af4-116">Request headers</span></span>
|<span data-ttu-id="c6af4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6af4-117">Header</span></span>|<span data-ttu-id="c6af4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c6af4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6af4-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6af4-119">Authorization</span></span>|<span data-ttu-id="c6af4-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c6af4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6af4-121">Принять</span><span class="sxs-lookup"><span data-stu-id="c6af4-121">Accept</span></span>|<span data-ttu-id="c6af4-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="c6af4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6af4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6af4-123">Request body</span></span>
<span data-ttu-id="c6af4-124">В теле запроса добавьте представление объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6af4-124">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="c6af4-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="c6af4-125">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="c6af4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6af4-126">Property</span></span>|<span data-ttu-id="c6af4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c6af4-127">Type</span></span>|<span data-ttu-id="c6af4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c6af4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6af4-129">ИД</span><span class="sxs-lookup"><span data-stu-id="c6af4-129">id</span></span>|<span data-ttu-id="c6af4-130">string</span><span class="sxs-lookup"><span data-stu-id="c6af4-130">String</span></span>|<span data-ttu-id="c6af4-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c6af4-131">Not yet documented</span></span>|
|<span data-ttu-id="c6af4-132">включено</span><span class="sxs-lookup"><span data-stu-id="c6af4-132">enabled</span></span>|<span data-ttu-id="c6af4-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="c6af4-133">Boolean</span></span>|<span data-ttu-id="c6af4-134">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="c6af4-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="c6af4-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="c6af4-135">includedGroups</span></span>|<span data-ttu-id="c6af4-136">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="c6af4-136">Guid collection</span></span>|<span data-ttu-id="c6af4-137">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="c6af4-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="c6af4-138">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="c6af4-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="c6af4-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="c6af4-139">excludedGroups</span></span>|<span data-ttu-id="c6af4-140">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="c6af4-140">Guid collection</span></span>|<span data-ttu-id="c6af4-141">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="c6af4-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="c6af4-142">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="c6af4-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="c6af4-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="c6af4-143">overrideDefaultRule</span></span>|<span data-ttu-id="c6af4-144">Логическое</span><span class="sxs-lookup"><span data-stu-id="c6af4-144">Boolean</span></span>|<span data-ttu-id="c6af4-145">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="c6af4-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="c6af4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6af4-146">Response</span></span>
<span data-ttu-id="c6af4-147">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c6af4-147">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6af4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c6af4-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6af4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6af4-149">Request</span></span>
<span data-ttu-id="c6af4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6af4-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="c6af4-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6af4-151">Response</span></span>
<span data-ttu-id="c6af4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6af4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "String"
  ],
  "excludedGroups": [
    "String"
  ],
  "overrideDefaultRule": true
}
```








