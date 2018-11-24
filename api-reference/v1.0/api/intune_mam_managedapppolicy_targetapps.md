# <a name="targetapps-action"></a><span data-ttu-id="f6770-101">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="f6770-101">targetApps action</span></span>

> <span data-ttu-id="f6770-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f6770-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6770-103">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="f6770-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6770-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6770-104">Prerequisites</span></span>
<span data-ttu-id="f6770-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6770-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="f6770-107">Permission type</span></span>|<span data-ttu-id="f6770-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6770-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6770-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6770-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f6770-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6770-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6770-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6770-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6770-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6770-112">Not supported.</span></span>|
|<span data-ttu-id="f6770-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6770-113">Application</span></span>|<span data-ttu-id="f6770-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6770-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6770-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6770-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="f6770-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6770-116">Request headers</span></span>
|<span data-ttu-id="f6770-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6770-117">Header</span></span>|<span data-ttu-id="f6770-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f6770-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6770-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6770-119">Authorization</span></span>|<span data-ttu-id="f6770-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6770-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6770-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f6770-121">Accept</span></span>|<span data-ttu-id="f6770-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f6770-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6770-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6770-123">Request body</span></span>
<span data-ttu-id="f6770-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6770-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f6770-125">В приведенной ниже таблице показаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f6770-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f6770-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6770-126">Property</span></span>|<span data-ttu-id="f6770-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f6770-127">Type</span></span>|<span data-ttu-id="f6770-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f6770-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6770-129">apps</span><span class="sxs-lookup"><span data-stu-id="f6770-129">apps</span></span>|<span data-ttu-id="f6770-130">Коллекция [managedMobileApp](../resources/intune_mam_managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6770-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) collection</span></span>|<span data-ttu-id="f6770-131">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="f6770-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6770-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6770-132">Response</span></span>
<span data-ttu-id="f6770-133">При успешном выполнении это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6770-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6770-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f6770-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6770-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6770-135">Request</span></span>
<span data-ttu-id="f6770-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6770-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f6770-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6770-137">Response</span></span>
<span data-ttu-id="f6770-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f6770-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



