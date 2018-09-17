# <a name="update-iosvppapp"></a><span data-ttu-id="b577b-101">Обновление iosVppApp</span><span class="sxs-lookup"><span data-stu-id="b577b-101">Update iosVppApp</span></span>

> <span data-ttu-id="b577b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b577b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b577b-103">Обновление свойств объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-103">Update the properties of a [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b577b-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b577b-104">Prerequisites</span></span>
<span data-ttu-id="b577b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b577b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b577b-107">Permission type</span></span>|<span data-ttu-id="b577b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b577b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b577b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b577b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b577b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b577b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b577b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b577b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b577b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b577b-112">Not supported.</span></span>|
|<span data-ttu-id="b577b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b577b-113">Application</span></span>|<span data-ttu-id="b577b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b577b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b577b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b577b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b577b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b577b-116">Request headers</span></span>
|<span data-ttu-id="b577b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b577b-117">Header</span></span>|<span data-ttu-id="b577b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b577b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b577b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b577b-119">Authorization</span></span>|<span data-ttu-id="b577b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b577b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b577b-121">Принять</span><span class="sxs-lookup"><span data-stu-id="b577b-121">Accept</span></span>|<span data-ttu-id="b577b-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="b577b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b577b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b577b-123">Request body</span></span>
<span data-ttu-id="b577b-124">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune_apps_iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b577b-124">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>

<span data-ttu-id="b577b-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-125">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune_apps_iosvppapp.md).</span></span>

|<span data-ttu-id="b577b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b577b-126">Property</span></span>|<span data-ttu-id="b577b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b577b-127">Type</span></span>|<span data-ttu-id="b577b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b577b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b577b-129">ид</span><span class="sxs-lookup"><span data-stu-id="b577b-129">id</span></span>|<span data-ttu-id="b577b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-130">String</span></span>|<span data-ttu-id="b577b-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b577b-131">Key of the entity.</span></span> <span data-ttu-id="b577b-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b577b-133">displayName</span></span>|<span data-ttu-id="b577b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-134">String</span></span>|<span data-ttu-id="b577b-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b577b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b577b-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-137">описание</span><span class="sxs-lookup"><span data-stu-id="b577b-137">description</span></span>|<span data-ttu-id="b577b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-138">String</span></span>|<span data-ttu-id="b577b-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-139">The description of the app.</span></span> <span data-ttu-id="b577b-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-141">издатель</span><span class="sxs-lookup"><span data-stu-id="b577b-141">publisher</span></span>|<span data-ttu-id="b577b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-142">String</span></span>|<span data-ttu-id="b577b-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-143">The publisher of the app.</span></span> <span data-ttu-id="b577b-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b577b-145">largeIcon</span></span>|[<span data-ttu-id="b577b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b577b-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b577b-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b577b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b577b-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b577b-149">createdDateTime</span></span>|<span data-ttu-id="b577b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b577b-150">DateTimeOffset</span></span>|<span data-ttu-id="b577b-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-151">The date and time the app was created.</span></span> <span data-ttu-id="b577b-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b577b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b577b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b577b-154">DateTimeOffset</span></span>|<span data-ttu-id="b577b-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-155">The date and time the app was last modified.</span></span> <span data-ttu-id="b577b-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b577b-157">isFeatured</span></span>|<span data-ttu-id="b577b-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="b577b-158">Boolean</span></span>|<span data-ttu-id="b577b-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b577b-160">privacyInformationUrl</span></span>|<span data-ttu-id="b577b-161">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-161">String</span></span>|<span data-ttu-id="b577b-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b577b-162">The privacy statement Url.</span></span> <span data-ttu-id="b577b-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b577b-164">informationUrl</span></span>|<span data-ttu-id="b577b-165">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-165">String</span></span>|<span data-ttu-id="b577b-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b577b-166">The more information Url.</span></span> <span data-ttu-id="b577b-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-168">владелец</span><span class="sxs-lookup"><span data-stu-id="b577b-168">owner</span></span>|<span data-ttu-id="b577b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-169">String</span></span>|<span data-ttu-id="b577b-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-170">The owner of the app.</span></span> <span data-ttu-id="b577b-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-172">разработчик</span><span class="sxs-lookup"><span data-stu-id="b577b-172">developer</span></span>|<span data-ttu-id="b577b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-173">String</span></span>|<span data-ttu-id="b577b-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b577b-174">The developer of the app.</span></span> <span data-ttu-id="b577b-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-176">примечания</span><span class="sxs-lookup"><span data-stu-id="b577b-176">notes</span></span>|<span data-ttu-id="b577b-177">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-177">String</span></span>|<span data-ttu-id="b577b-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="b577b-178">Notes for the app.</span></span> <span data-ttu-id="b577b-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b577b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b577b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b577b-180">publishingState</span></span>|[<span data-ttu-id="b577b-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b577b-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b577b-p114">Состояние публикации для приложения. Приложение не может быть назначено только без публикации приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b577b-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b577b-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b577b-186">usedLicenseCount</span></span>|<span data-ttu-id="b577b-187">Int32</span><span class="sxs-lookup"><span data-stu-id="b577b-187">Int32</span></span>|<span data-ttu-id="b577b-188">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="b577b-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="b577b-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b577b-189">totalLicenseCount</span></span>|<span data-ttu-id="b577b-190">Int32</span><span class="sxs-lookup"><span data-stu-id="b577b-190">Int32</span></span>|<span data-ttu-id="b577b-191">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="b577b-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="b577b-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b577b-192">releaseDateTime</span></span>|<span data-ttu-id="b577b-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b577b-193">DateTimeOffset</span></span>|<span data-ttu-id="b577b-194">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="b577b-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="b577b-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b577b-195">appStoreUrl</span></span>|<span data-ttu-id="b577b-196">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-196">String</span></span>|<span data-ttu-id="b577b-197">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="b577b-197">The store URL.</span></span>|
|<span data-ttu-id="b577b-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="b577b-198">licensingType</span></span>|[<span data-ttu-id="b577b-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b577b-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="b577b-200">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="b577b-200">The supported License Type.</span></span>|
|<span data-ttu-id="b577b-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b577b-201">applicableDeviceType</span></span>|[<span data-ttu-id="b577b-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b577b-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="b577b-203">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="b577b-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="b577b-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b577b-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="b577b-205">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-205">String</span></span>|<span data-ttu-id="b577b-206">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b577b-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b577b-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b577b-207">vppTokenAccountType</span></span>|[<span data-ttu-id="b577b-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b577b-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="b577b-p115">Тип программы покупки объема, с которой связан данный токен программы покупки объема Apple. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="b577b-p115">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b577b-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="b577b-212">vppTokenAppleId</span></span>|<span data-ttu-id="b577b-213">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-213">String</span></span>|<span data-ttu-id="b577b-214">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b577b-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b577b-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="b577b-215">bundleId</span></span>|<span data-ttu-id="b577b-216">Строка</span><span class="sxs-lookup"><span data-stu-id="b577b-216">String</span></span>|<span data-ttu-id="b577b-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b577b-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="b577b-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="b577b-218">Response</span></span>
<span data-ttu-id="b577b-219">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune_apps_iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b577b-219">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b577b-220">Пример</span><span class="sxs-lookup"><span data-stu-id="b577b-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="b577b-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="b577b-221">Request</span></span>
<span data-ttu-id="b577b-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b577b-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="b577b-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="b577b-223">Response</span></span>
<span data-ttu-id="b577b-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b577b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```








